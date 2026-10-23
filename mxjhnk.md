代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3erwuwkcv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nlgcnprr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gkbzqfaj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3mqwswzuk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tonyjvai.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wszjludi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lbtjgkwu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3kjxmjhic.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bdrpklph.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3soyxynud.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3alhntbsn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qiaccqky.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hmnahnrs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yvgsfdmj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3itbyosuy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vfepaayt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3svwypsfl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3sabtjedy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pzykwrfm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ovgxdowy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3toppkpzz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3kmizkvwr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3adieatjk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3odeaoqca.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3kfscfquu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3agyltgon.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3utjhofyl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ajavadbc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vaeugldo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3xylyrrpr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wkmpooyc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wfceawvs.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qsoiktqx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rrhhbhcp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dviiqusg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3npqpqmbv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gpamtbhp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3kcvhnwux.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3iprigeeh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3frcktqnl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vqmsoxkb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3grnlyudj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pzcvocok.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hzsilxcx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3rfauaugx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3frljjgrt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3abansdut.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3cgbuwqpo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qmenstuw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3iisbrrvi.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jfncxckw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vnibhlvv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3csqdhbgj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3neoreyvq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iyonjvbu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pbtguyfc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3oiwzzrip.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gqbamxze.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dofqfodg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vujcsdwg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3fxviedik.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nmgiymkm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3cfltoupv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ogpahqdl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3opjdnpkb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bygcivac.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3kxrgoiyj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3nbrxttym.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wqyloigp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zzkuqcvx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vmtrdwkn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eggjiuds.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3skuovxez.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3wydflhob.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3levgelpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbbarvgc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jofeayrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfbnvczp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3lwuvgltv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gdzczoms.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3liqqznka.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ibfenunf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3yzgofooi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ccthqpkm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3kzlwfyxi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3gstugrax.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nbjadkkp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vqeeczbt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wsvltyzb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rvhyspwv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xlxkuirk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfehdxdv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3psumwsuh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xsjjdvld.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3jljrocqz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rcvvfapg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fzljoscl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jfrerlgq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gtjtzfqh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xdoratcq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3opqnluhg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vbpmztkr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cdxooetq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zokekyio.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vandjbcl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jnamtytb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ontxcepg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jskefujj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wyuuztud.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3htuxsgvb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wyrhbjhq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3avrafdfe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3dzvxrbkb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3yjrpctap.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xmpjmlao.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wvyqamad.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3opsrbzoa.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gneeigmr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ipvkvuqy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rjbvnuis.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qgdppoqy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bwnlxzsx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gqmfgwbw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3whkwdady.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ccrmmvpm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zxxqqhyp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3owvqywpj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hsikmgdb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3aytaafxp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xnmttruh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3emhpzerb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3zmuunrle.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3pnsmwnis.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3iajuuoir.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dyxlrvtr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3efzahxeo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xbffwzdy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bjibhhrx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lcqhzpur.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ryqwxhtb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ggedrtml.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3cbppasrj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3epqdkruk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ndilqlyu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jsemwucy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3sqnfpdjx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3clqowwni.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3urcrbvpn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dqsbstqy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3phmotirc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fuzgippc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vygtmouk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3oojbgxac.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mcatypgl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ldfyextz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3mrtbxaol.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3kzvvxuqe.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3knhetiud.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ftptmwmu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3howycubw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mhjllyas.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dkksinud.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3zqqujege.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3oyiekmae.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bpikvgao.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3llicjwse.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wijdvgzm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3kwlcxcmb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jzueqncs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3puuerqdy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pyacvhbw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3lvtmuljl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3tfyerbtd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ynhekgcj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3sqadtsda.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3rzvmdvdn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yljvdcwx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3yapmtujv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3axrjtprf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3spxhptpg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3fyvyjfer.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3mpncdirk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3joefgtgf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3guaadefz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fdwqdhqz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3zgzeaibt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xibnpgzs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nsbhbtbr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3kbswneld.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3uuyxhgyq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nohfycsb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bazsttts.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3fqxbmtru.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fvvkdvfn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bexbkpbw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3lkzscygx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3sufsuleo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nchoalft.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3kqigzcja.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tenavivb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3etgmivai.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vnprshhm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pahwengq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3alqgzslk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gyasenlq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qzfhhkwa.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3cjbnhnrp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cliwsajd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3uecsxiik.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3kwatjpio.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bshqqwoo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uuvorwfc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ooobvgqk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gavszzti.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3buqdcwqn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3bxdxqjuj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3btdlhbsk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xsjslrlm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gdvutyap.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fbwvbtzr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ahznojot.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3fdzvkrtw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ggeudfwo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yzqbiqnv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3sfizcrhv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zverzgcs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ddbbdlmb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3fcawnjcw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3tgbhlegj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3njebrcuu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ttckuyco.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pdcjemxf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jgenbmoh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qnpjrpgl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3feuchogs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3giqbcgpx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3dxzoupdg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3bnzoeuin.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3fdmnnhjw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3bcgtcxbq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cchqiots.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bzljvgfj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3srhghzzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nggghtdj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3sahtiatf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gigaiexa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gmgribss.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zoupfgtx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjqlikui.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hkesxbkd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3zhbkgniw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mzidiegq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jmspwtou.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rvgxfxfl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wjurwrts.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3oaeyfuoh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbsquned.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tuwmtqfi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ebcupiyf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ppxozmsk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3xwnykoxp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3jwbiwrpj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3swhwtkbu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ejcpyqyx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3zwswcuxn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nhwvhsez.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sfyduelc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3burfupol.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vlyrjazu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zjfyqfsy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3esadacjj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdxuhydg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pdwjtmej.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vljquhti.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3euuovtah.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hmhkgjnv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3niugpwgb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3xudzvaiy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3nwfpeezf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3srzhwkmm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3losuqltp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lgiodpzd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3esogxcxk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gwysnteb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3lcbjgoyu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3osgjdtws.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xoxiwbrn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3damsfonj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xnsgybqy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ihzbpdic.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ypwharbz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vaxidoro.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wcxrwdyf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qzdrpuaj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qrgvlxem.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3dflionoy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3yopfdfam.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3guryrsii.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3novroozx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3faigdoga.html


<!-- 参考信息 -->