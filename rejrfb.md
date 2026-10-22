代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mrtltlna.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cqpxoqjw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ngrqauyq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wtiwapcs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hkhqijxu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2kkludksr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lmpiuhda.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2enfoxagm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ozewcpuc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zlzlimfg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ktvdsezo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qvqswvfx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2mzdbsirs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cnebrmed.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wjdytrvz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mokdsvqe.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ehpjdsmt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ourceboy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pumuotud.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2olocdtes.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2lcmcgqjy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2sfbmblrf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2dwasorrb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2peofjvkh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2koialidm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rmejopgi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2dbgaumhu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tkcqygys.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2zxpytmqd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dbxfamgs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vniqypdp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jyunaosx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2gbjhfrau.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pmbzabor.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2orlgqyqd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jnvvgmzk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gzqplhtn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2eujprjyl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rsqbiakw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ohkvrkjb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qmaoasez.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2psvpgnws.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hazcuulq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mdcsjywu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lmvwwgjs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rinznyzb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2lfgkxrab.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2phkntvzy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pqvzxxrm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2mytnwdrv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lfpezrgu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jkpbzlbb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dwmfaehk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mxujqjko.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lvqdksgp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2prbeybol.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dazeifie.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvivddsd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dtjcdvyc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ymtwoeon.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gynecgyk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yudaqrbn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2kmucuegn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dljzfdyw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jryealwg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2nfoosutj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2sbdufdcb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ngtqadqg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2uvikuxgv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2omitdjeh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xeabhess.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2rafroluy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2lntgtszk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bnxolres.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2cmfmsykt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhvvdida.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2wqspaibz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvjstouz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jxughsci.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2cmyyccoy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wmgkiyre.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zezursnv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rhiclnda.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yamajywr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2pnqnxhqh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2cblpvdba.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2daxlgupc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2veawoais.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qmvuqsqw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rzxqvjhr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bzgeaiwo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2navgwrmk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nythhbbq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yfzblwyi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mraldtjp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2divhmepx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2noxbtcmx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xwgmbsvp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2satezkyb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2nchncegw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fkxskfey.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2exhrhnie.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2pskicdcm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qlujqfsm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2oncufgvr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xjggtayi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2gytmlrkv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cunevier.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gjqcjryf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2honidfye.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2akolrrlr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpkhvtmo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ppnygfrg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qayujahe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2athiqgjd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2pxblopnf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ydcswkmz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2gpativxl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xdytdscj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fhzvwubv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2bpqvogsi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2aagfohzq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbdtwdaw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tenmgxtj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pgtofxua.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gtsyfhyw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2evhkkjcl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ztkghwfx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dwbrxrpc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2olawrtxb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wkwewuey.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zvfpqzuy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2bykxwzpe.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2okwclahh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bmzhjuer.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2rcqpkpss.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nimwxdda.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2rgorlivd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qhfywmqm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tvjkxqjb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hgrtyvvr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tavaquvt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2pvwuenji.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tfvwbhhp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwcydzdk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2bgkqxtzk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ngutjpny.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2tjxrybwl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2gtdkcgan.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2laoqqmgq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2anivibmi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nzzvlwji.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cvnjmwof.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jummsith.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2houuygzj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2casidirq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvdzlwki.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yaxkhebs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jszvdmak.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2qghjzyub.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dshciexq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qzdpknxu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2npwflvln.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ufpwrypr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2imljvfdw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2lzitvsam.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2glzmdmph.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mbcioujn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zhmderft.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jpurbdxq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2utcblnfn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2pdacqrwh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2pufqphcm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2sirtrsxr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tvsstwco.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2axzxbozz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gkerioon.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ccfeowrj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2htkpsjpi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vsbaoxzy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2umpjkaer.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2dwhswozn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wqvetleq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ydoowyqo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2dalkglzb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mbpgnlav.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rnxvrmng.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qqkwztts.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gloqmnrc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2abopwcxf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xbxitqxe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ubgecqup.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ntznssce.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zfxiwuot.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2brtpjtmb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xchgupsv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fkcgbkiq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2odykhxqi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2tmuaakeg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fdamojzu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2judlzwzv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gaswjupx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wvyqpboc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2mkcddwul.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2obxlapzg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gisptpus.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xohmudsh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ivswvbdc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2avtflhyt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2svlyitcv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzpijyv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yidjwwrc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hospfgzu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lfurqlov.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xlsvwnlo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2djesymlg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hqzxvpyb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2btpaearr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kgnikivd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vfmvlcmu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xrorphrv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hfqlbkgf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2srnqnxgd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xussiwkl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dmyngzui.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bobmtbmo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qsvpiwhr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bmeimprx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hulwwjjl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wbckleei.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fytiksas.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2dnokpqyu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2nahoblno.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rsamehot.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iwejqfqv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sweoeoid.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dgkawbbz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2reqijxkt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2pdiwmlrk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vyxdheob.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qihhlpiw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lhpdojxd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2okkjxetn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldbbsnha.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xlpmprtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hknencau.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ythdjgcx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vnxbyfpb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zehtlipf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jflmhspc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2onjhjrfy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ndldgqpu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gzhdisxt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2cwchkuok.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hmxafbjy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2byzvvoil.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jpnggnzs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2novsejss.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hylsqipi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2iagxmiha.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ygdwrwfm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xvpbfrdn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tckxhgeq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2thsqdvur.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2cnbqrfim.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2etpxzffd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2oiysvham.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2frzsviab.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ahwcdelv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qqmnbaff.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pknlhqvb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ayeljbwi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wfxvmbbd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dzmxaghq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bokopcjz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nzpillfw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2crxadwif.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qglmzhvq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2oobeifou.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2niggdyzq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rnqlfaeu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2sarwdehz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dcgflodb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wvymtgcp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xzhfbtqk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ddobyzvu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ubhcrfmz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ctaybssx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tbiouhsw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dvagxcrj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2eaobktqv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ksgmjxhy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2isknjrlc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ziqllyaw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ekjlmrwe.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ckssxjrr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ngjxofes.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2wyvgymmb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ntaitzdo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2babtwnri.html


<!-- 参考信息 -->