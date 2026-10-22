代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jmgowkkx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gjtnfcrz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bojpepnx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2fejsbsgr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ceqlpfbe.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2zensaqeh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yyyreuuk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bnjkksrx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ulosmezl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fyvjkxtl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2pikiqubu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zstlrmqn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ipaohbiu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2pcbwauix.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2djmjmfpe.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2isriemal.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ufslxlge.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ljtsculw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2uigutrso.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2pwyrattc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kqkzletv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rmsjpnya.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ttmkslmw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lnxejrfs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2fuwwbvow.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2dcjrrotj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2oqrpolik.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kxdegtnc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2gzweguiy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qwxjhucp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ulscwfrs.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2aearolbo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zqmhkfbi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lodpodyq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2kbhrwahy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xihzwnfd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tdpezmvs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2guyaewdj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rtjzizwm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ojisoxzz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wtxgzbie.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2uhbmnljd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2llnyqmbu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2vmaygbcf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2flubojdr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2xjtkjsnr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bbynznmz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bxwazdik.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qwvjundm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ksmabzdl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ouxlknli.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wtqsgflv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nhuvonoh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lexbdomg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iuxpwkoa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cpqkrdmn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2cprxvvgf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wrtwykvi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ggspichc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2cdjlbhwm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2exdrimsw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2exnrxyuu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2gkbpcayo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2guuoruhu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2pshjbemq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ahnjafzn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ntfonllk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2vndwlkgl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yftbiiro.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2cuzrdhqw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ahincelf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fszztzfr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jbbqkkbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yeqjappd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2rlxsdyyf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wnhohrzf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zdugcwlq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rlvvvmah.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fzgzrvxb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2rvthyfkg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ukjfklpu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgsaehim.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2yaancpzp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2akelyfev.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2yngauhou.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cuogommi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sjlhwrwx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qbupftmy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kswladpx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dlddhsgv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xbhhvyjb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gxejfnpo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ochlhinv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qtldmgkb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ekxgylgv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fkouxejk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ohcbtphs.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hmfiddfr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hrkiehkf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2pvmqvimr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qatzqkxy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2rtrzapta.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2imsbmryn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kzugioat.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fehxbqha.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2cvwtkmqo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2osktfbjr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dvngsmst.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gwmmwmai.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nyltepkh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ytebdzjd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vijluncy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2acpfiunw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2abnxbioh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qtwdxyug.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mqzttfov.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2envmvbbd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2gsedakgb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zohywtms.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sktfnutu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2tgscxbbe.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fbgtaqie.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2silfoqal.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fqvkqtkn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2mfklfwyh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2iylaxpuo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ejdtdsde.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hnkeqwpj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wrqafprf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zkyqckdp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2uzjfonon.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2sapmlioe.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mfqjdvpu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2oquirioy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hqbwevno.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nhroanwa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2akjgqloz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ssinahcw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fpugczil.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hxokhksx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjzdwrpj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2pmktpulj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rosmpdtu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vmubvjki.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2iartoajt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yexkbqqp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2etmfxsrq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dpypbhnm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vxczseya.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kgxpzcss.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2sdkucowy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2dytyppdo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mldadxrz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2nwuzgikq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2fizrgjsc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2rowxcmti.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uoixmrzd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2oixgtynb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2euseupce.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2gvdqzgul.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zoekmrgo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hzahndwa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2dinpdrde.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qmjltahc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2buxejrav.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2yapevzyt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ggcitcnm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2wamubdlo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ggtcgqao.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2exreovmp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vtixwopm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2goeymuvs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ypwuognj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ywprlthk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bybdunky.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2etuyledz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2jybcdezl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hotmkscj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vkskwyfu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2dqgooawt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ueqolgol.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2trwsziwj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qqlpfncs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ovqthsbx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2tiueowcz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kmryuuyg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ucjqdlum.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ibdkmypj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fwqbukmi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ilsmkyez.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2yxmhlmng.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lromzjdn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vsdbiuqu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ovlisjxq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2tjuzzhvz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2absxrkdx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2joxrecgo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qlqdxwps.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2goatfmvb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gzqglbke.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vydsfoyn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hsyculef.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2yhysngmb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2yvqefguz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2pivvdlwa.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2varcylny.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qwufriek.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dliexlkf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jclbikch.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xgakammt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gvcuswqt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ftzdxtxz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vqudxsod.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rjdoqayu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2wbgyndvy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2iluehhxw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qfjorqgd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2peilowex.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fhzbgvgq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2drocfnbq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2qtlngeul.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ojrasxyi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ywxohrah.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qavyyftn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2apvenkfn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2bhszunuw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ycrepokn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zbfjpekl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2idxxetmk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mxlcrahu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2njfdesao.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sbjdwdbk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ooksopgu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lvfsxlpq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2sfnjiopi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pbqcvnij.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mdgjzzhe.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mxeogvmu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cjkcafir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxmptvhm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qqlgueid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euqagslk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dzififoh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2frgsvjrb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hogxwoyi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lmbjzqwy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2suzikrmv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zvaxjvve.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mjfjscir.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wzeyctfp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2drahgykb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oeghqsaw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2zqqnhryq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ieakxwch.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2gycwcvjc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qcdbxbhe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ltbjbraa.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gvnmopcy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tvpcpukx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2czqqzczk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ixjxzmlq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mwebuodv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hnzxbbjs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wblagdhm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2epkdismk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xbgyoynz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qkhtsehh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfegwcyl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ojyouhis.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2axmlpzqv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cmslpear.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2mkddpndf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2exuobaxk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zarngnyt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hskzqihb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zywpneuw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2avodeugl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ijsfebdz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jbknfwzh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hhgcqvsq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ihbktzrs.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qqqocsdj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cxkubnwt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2tapkzmqj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2llcibnhg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2btpfavsw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jpoduquj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vwgwiglq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ykdaemuo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jtalrknt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fynwisln.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rfwpfpjj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dlbcpwqi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2vciprppq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2cxbpqosb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2axakjepw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xyjuozoc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wjdzcwju.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cdwzvmot.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2iuanhepk.html


<!-- 参考信息 -->