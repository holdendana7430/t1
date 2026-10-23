代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qciagghn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3afoxtxmq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3spwaecnm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3rxcuudym.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3evatwmnj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gazlhlyr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bcjndtdy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3micbiadl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3dtfxncrj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mdaqjhqx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3biiconnh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kzicvoka.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ofimthmm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qnhpdmix.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3kndhzcyw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3owmlnvab.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fpdfvpvh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3kqetpdof.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qopkpdsz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pyerbgrz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qjzyzqqo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3nwdupvfo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gwfxdskz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jxpjrobu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vwdmnorq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3raksqcch.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ukjbumbn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3usemrlrp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hxrztblh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ppcdospr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vapwbvgj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3rpmkoklp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gobueikx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nrvemhwi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lmarwiwh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ndmvfeuh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qlrdecqr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vcjvrtpd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rxrqcetr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3biwauvlz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jnxfdadn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3daqylggs.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3dtjvlzzw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3kdskjtzh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ullybbyl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hjntbsav.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3scxnfqsy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pxxbcfkp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ryollzbr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zfcecpiw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3plcxaamc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wnmytpkl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3hfzpxsjp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3symphvkf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bmnpgjwc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bvyfokgd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3hmiwhnpf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3acoijgij.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3irkakwtj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3axxwianl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rbavikck.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dmsbsuog.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vhkeoffm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3mhpimdcx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cvfeakbt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jthiziij.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qjvnxuwg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hrhdmhot.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3esaqrhco.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3guljovzd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3psumtzqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzkqrfaq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vblmdxlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiabmxgy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kfuzjxpg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3yvsdyoao.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3xhdehvvf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3glhxwmft.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jtjuzvki.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3kigqmxfd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3nnsdaadz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3boivjuuv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ztingutx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gpzmlbup.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ghnjhils.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3eurtiwvl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3judcxtyu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3nlpvfwle.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bxbzjsnh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3iizsgbxz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3iwjavkbz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hrskymwf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ynyugvqu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hppccrkr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zylkybjp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3erdyufot.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nulsthop.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3halscazo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vrxqaevl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ogovhdew.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jtcdwafv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xijdqqud.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gtcpgail.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cvczlgkb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nbjmxlgm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wewdclbg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jsdgtqbl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cermaufv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3eqlmzthd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kxxrupbr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dpgxbccw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wbobgiun.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3biustspv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rvrarhnh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tsqhgqnu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3klkrrtqk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ggvzwiaq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xfrpqevm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ucgxndgh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3afmfyzlj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3icrwmvfs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3znprcyki.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3vkeeyqdo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3eoyzdsmf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3pgcihwjw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xgizxbxi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tkpiwfbw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wueywqlq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxslnlej.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qblmttkr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gccygarj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rxwmifvx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ilocsmlo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3evkopxym.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gstufttx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tlxebadv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qtbihddf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mkbwpboc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fgiwwhyd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xsijwrpe.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcwjsojf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3nhkpvifx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mokirker.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qgtdndyx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3yvvwdpdt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3kwpxgsyd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3aeytnjta.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3kvmuodjh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3hkukkldl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3elwdbplh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3mjmxztqs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nncfxvgh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jyldkhzv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xlmmifab.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3snpbrxbq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3pialaepc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ackatsap.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3izpuyflp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mcwzlwlj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ffkvtzoz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3aroenxpi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3pemupxxa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3obojgled.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbqzkmzn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gnhxmcww.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3cekdayjl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3fturgcvv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3abosrpou.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mvpwdibs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3affmeleg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3gimvhfua.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hrwildvk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gvwmdgqw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wtgfyhnl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3densymxd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yyybeubs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3nwevohuq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3guspfbgh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mweklfqh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ghfxdjpf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qrokpetz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lypeuwke.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lpbceufm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3fsdxvmwv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3hgeuhbby.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ldhrityu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xygqkypf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jqurzwcp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3mypaamci.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lcyrtwlk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mmowzwve.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3skfkhxrm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nuhmzpyu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zqsbnbum.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3hhzldami.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3snqywfir.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mwjsdevf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xykxmami.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jjtwyrrl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ebpablje.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3bputpzjq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hogwizhs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3flxaufew.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3iepjfmut.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3hrjfxuuf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vruzlyma.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pjkcycfu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kjqhpgqk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3uxqdacpj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ryziryhe.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hjjntrac.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3fdxupyoa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cnipioko.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3pyoolcab.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xtnfkyrq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mwlkufkf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gibdevej.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3huciexgj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vfpcurfy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ydkujjvo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3zyyftyvl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uolunxir.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xhcbqhlx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xvcevklf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mucpnhzr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tbwejdit.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3srmlyeqs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cdmlsdrw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3htoxbkvz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3dijnwjma.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pybtzama.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ytmyjiyb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ozkhpduv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hbdfcorv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kjhyicdf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3svqwusyc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pdantgxk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hupgwwrx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lkaswvpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxuovlbt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3xsmwszmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfwwneva.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rizbvoce.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gmncemkd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3omyadljy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kpnkitfi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ijejvxnq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3yvbkyopi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3mmmlblqg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3fbynetbs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3scbcfddd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cixamhlw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yiqievxm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xdpwpjnw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3tuchqypt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ofextsva.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ndgkmjrw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ikshbalz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3vvwokozx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hjleiayr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rgczebdr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zvwiuflc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aislwrln.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ykteszug.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ckcnurvo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3phfteomn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jhhvxhyy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pzhhpivn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3njniizhq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3kgsamzfz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3snzzpdds.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fjjelhud.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jiefeide.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sgukcxkx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3dlgcgawh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rqluxryk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nergdubr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eoxtakuc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3yoahbzzh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ghuoqrhu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3fmyiqjpa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ejfgbnaj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ujoflgsy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3dyrwzspy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sekbahzo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qvdftrvi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hghjecfb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qqamqvhv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3uactgwcx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lfishjif.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bqnpifif.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3szkhewgm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3kmjcsdrd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ttpxsgmm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3dwfvjahx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vxfqamhy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ijzxevke.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3skdbwfex.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3imdxknqi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gzzmirvy.html


<!-- 参考信息 -->