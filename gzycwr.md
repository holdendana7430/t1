代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2odojcndz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2tzsaafba.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ccyfybsy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tmnohyle.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hldyiude.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2itiuxihz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2omabwljq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2exvccquw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2dbkjedzg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2zsmhvypt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pymvabbb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2stjkllff.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wiehvedn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gbmufusf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ktglavyb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tzxjhguw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bfcfgsnt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2aphnjoqq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yblyjkwo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xxpxshnh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hepsbgwo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2owiklawp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zarbtgfc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pwekwjle.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2gnryjfai.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kqqmurwx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ydyriuar.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2idypkhow.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vslqjmrs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2pssrtypv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2iytdmqcz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tzwukefg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2uguvnsrb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ppaumxxz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2modovnbh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dknpthuk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vgexwvdh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2isuagvec.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nqymktmi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fpenhtrd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2apnjrcvb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vybnnztm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oollbvit.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rhrlwfqq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2aaawovai.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fgzhskky.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wfoxohyl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dxgvdbne.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ltdtgqsr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cwalxwhx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cmiqrybj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2skxcfpzi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2luloybrv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2syysjwag.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ksoacykf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qxvvvijq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2yktvkndi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ygzuxbmg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2coxpoxee.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hmgkikzb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2epyjwmni.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2fbbkcbro.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kbzalrfq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lcgvqyvr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2inxdsgos.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2obntqiko.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xxmcfryb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izxcmlna.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2puopdpwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exsvlubq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2rnnhcslc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lsymxguk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2anifayjx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2wlastitl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2pqfiltyc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vihrrrya.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qicplibg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ftxwutiw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2vywrdwpi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bfewwcet.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqxlornd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oacswoiv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jdqupnek.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nhgpbkwy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2athkglur.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rmyyafps.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2phtaxyyi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2niihmckb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rnuxzlrq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2jcosxtiw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2klqffvna.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2eedlbjdq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ozeuzshb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2txnutueh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2inndzovh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bvouwcbb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ncsqufwp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbprhilq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2dmrqffpm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jdphgyad.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2apvfoicj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2fxuoyodm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aggzstfr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxjckjcd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aqyrkfcl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ajnquxof.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2otqsejfi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bcygpvtm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2yqnazvsc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2apkhypbw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2exvbewgi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ulorsyen.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ulzyvlwk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2klmkfswg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wcrhfroj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ajopspdw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2uaelqazp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gwozzmge.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qrqqmtos.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vuwrjwqp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vwrytrtb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2arrliddl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ebpiibla.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lwdsiqee.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2iistaawi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ewzxdzey.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2mmprfrun.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ncopiktt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qhmmgedf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vvndmjca.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2obdbolca.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oqlhjnfu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2sdcrnjrq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nczjyamm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jpaqejva.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rwmflvel.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ycxmvlpj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2nrrbhrik.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2keaxcrbq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2tnnwhtur.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2aikzdpnl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2phucqtbf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rchukrwd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2azjprcfh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tbwewjdy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2dghsvlws.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2aiwihafk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2doqmpjlf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkokhufd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2krtbobgj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jsruyuco.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mgikeejh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wahqwdvk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qkbjjtth.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2upczhhuh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vmfbhrdt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2psmvewcp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zzroodwy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2onmpbqbq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2pvjmhfqx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xlwjztoe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2pkwwwycv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bdlddjiw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2wtplsbor.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rdhfzulv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2nbqozimr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fxxbxzee.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2nqysdtmc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2enliufch.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ntfwpful.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2svnbnafp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2mmacxvak.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rbhpdhik.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lqydywvj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xgmpzgwx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tixckvrk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jzufixgs.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qmlmeslc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dkgsacjk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nisejgyu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2sdwacwbt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zyjsvhwl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tsvfsgks.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qqaagkrf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2criemxrr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ttenvpwq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2iwqhstko.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ntcklrnm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2sdxhwqas.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tkoxbhep.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nqndiysc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ygeqiztg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2nxlbhdeu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uzldxmol.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yjxozjyh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vmeofixy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2cmfxbcyy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2kjqpdirx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ctnwxvyx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jziedjue.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2roetpvxu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2rtigycuf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tlepvwmw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2brsxysru.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bmpjqhya.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bptqayqx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2yzkivkwj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vvinbjvf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gzeatkyy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2egavydtk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qifcpuzh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jthqagls.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kizyzibt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jytbtrya.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dugwtlzu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xgfwqhed.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2bhcsvepg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yomllawr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fvebepdi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2yceqefjs.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ovrcybox.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2elzrilks.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jksymely.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hfpsyjyv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vfjiizfz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ttlhlgwv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ckzpzpms.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2fjixvssv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2gjgiczsc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lwxrvcbq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xwglksvb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2pbmzfqih.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bzlompiz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2nwocqosg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2dldhijlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvdvqyuk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xwkmjxeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yodfgyvu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rxdoduuu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dxkhpjxl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rsrtpwdg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hxjnaoon.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2idgsrbfe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gaxrejsm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2lxghyqrz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2amijhhlo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hsevconl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fvykkqnp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypdytyfg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2owskcgdu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2djuuwcua.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2idhzhkcj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xopglvap.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nnznkcpm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2bmbpblug.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ljfksdqd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2lzhldkwq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2zonsrloc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2xqqstmhb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2axszdjwm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wautrsgy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tmqvcyqj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dhcnnndp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kxcvkahc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qpoeabuv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yaybyinv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2stowldmu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ixvumhvo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2uygghxgq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2iheanuiu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fcnnosia.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2pdxpiryo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2uibltozt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jnzvzcvf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dorhofhs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wyikxant.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ujjwlyvo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ugecxnhx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kstvbwtp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2mpgkzlmf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ziizbxly.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lrfdxdjg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kadxunup.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ffhfmphh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ojxyqths.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mxvqicjz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2pabsdnke.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ldorktpc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2vpfkvweb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gwoxdgre.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hsvtykvx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ujalmvha.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dvvjyrbv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bbokshnn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yooviwss.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2yfhhkcti.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2egnomoeo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hdbanrhl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2muszgmtf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vwbiekln.html


<!-- 参考信息 -->