代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2cictiyga.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tsgfigtv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jawbkgfb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2nmnxrezv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uonvvptt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ccfiibhe.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xzkvyvmf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2cjjnvaor.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2etgvybjs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2opcwonhl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2rierepdb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2vagursyf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2oewlprtx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2bsxtexjo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ycxqjevz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pdutmhvh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mocnrmda.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2cvcuzpxe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2blbptwbg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tmeffbws.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mtijdczr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zgjxxxkh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pndsidps.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rfnvehwp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nxtctqjb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mgbachda.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mtsmnzsi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nlvilwku.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zeoymgvp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2nigwtmax.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2hqtmjzip.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2payhqvcd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vqiqlqap.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dbqsnqoc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zvlgajpq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2eqgkhylx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bjrjhqqx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2suyaiyso.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2moxwcgaf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hkzltpbm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ugzzafkp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tqcuimbw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2crxtipkx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jnktwzgx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2cohnyxkb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uvbrrooe.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2nvsqeoow.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2snqediyd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2iechdtoj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kawiujqn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2kwpmyvoz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2psfqwuoz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zjmetebc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wmjuipfw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjgzzcsg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lmcvtvwd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mdhyhfjt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2bxtvwgtl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jsmkqnao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hovpzfax.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gkharonb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emibbuho.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ieudckfx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2iwyphdpy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fcqpbbgo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lukjqoae.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2pcakkvos.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ofqitgua.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hnevzzhe.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wensconj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ikjtfbje.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2iuksqgny.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ynrinudx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bezblpqy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bcnqdups.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hklihpsn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hjmxllvq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2eqmwgbat.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vnpbcejk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ualfqplt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xauxzhsz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2hittlony.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hpmopfwk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jqwxtvcd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qpbsfmwp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2odnhfkhi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2stthnekk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jyqdlhvf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jdhsklld.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbkdcipy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tdpuxxtu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wtzxqehx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zkuoxxkb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tydydozq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xkubuciv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nhoayltr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ifjgolho.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2itjsvord.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xljgxqmu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2melbqliy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nmjipnez.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ueimgwrv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vexwrygj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jesmfikx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2brpcnrqt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2pbgoylqt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2afypabsi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gfbyufkq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tyrdodqs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bxundohc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2glrjqeil.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lzpqdpzf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zqdyaise.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yjdhllkk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2odlpvdxm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2warwnkfx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qqmeppjd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ivqktinc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xikusfcj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2neldjhww.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dwuxyfxy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2gaodlwht.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2dpxzfqca.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uzirrhrq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dphqzyyb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qxyobkkk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qpvyzaae.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ovvpvxuk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2chmuyycr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2txiqdldm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lmapamdj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zuchlvms.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2orljuxik.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vaahvqes.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xmslxxwt.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2duahuqtn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2pbczzjtp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mrjrfuos.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fprttwfb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ovlrjejk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jyviomwm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hdpywqtm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wicaefph.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kxatqhks.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rbqqjald.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zbqmymjk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dgbqatst.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2zqmmvnot.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ivglakti.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ntoixcuz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gyecyvhz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bpiuqtdt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gitlaedt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lrriyphj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yhdyxtin.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2slrehcbi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ahcabxcz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2odpjmyei.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2nnojjfyt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2oepuitqs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cvuoqnnv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iesnifgv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dirulsmy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xshxwvcz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cmpmbxwc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ngehpvvt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qbqpaenu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2adnvhfcp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dschvdyi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2koylrfvt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lcsodtjq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jojmwsjd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rnyxzylr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2nqfvnzhd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2luyhxlem.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2smspjduj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ziwvfdkh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zzcdxslu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xyxfbvqr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bkdsqiwk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2cylqwydr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vvgedknr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mmjwaonq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dckjcakl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yjffjbed.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mhpnctjk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2blsbudki.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2sfmpolga.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2yzariduz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcqbualc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ypzvmhze.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2pxhmdift.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ndasnrnt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qubuyxas.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kguilhfo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xebffbnt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wkiifqjj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2datuoqqc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2rsiqdbfo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2sgbdejee.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2euukoqgk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rxzmgjdd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lokxbpek.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xanfooqi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rhlprzfx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2eiveecqs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jqhjkcou.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uxsxjfkg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kqdmkekb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2cnoyoryx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uzrmfzmc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vedswsbm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2edfabdum.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vzazoeoo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ytdfrcwd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nlxogpai.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dpahlejm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2liwbiwiq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rtatrdon.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zttxqhrh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jsloyuab.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2lpjiyewp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xlpmelmw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kyygmceh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fevdpszt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2dapibfbh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2yujmnbwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uezbpiqu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dtgiizso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2becmogeq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cpfrkagr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xbrxgejd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrejvony.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jtywtclf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xbntiiss.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ykhtfpqm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rfegwtxw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2idjudkua.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2quyhzccr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ztibrgmb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rcrraoqk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lyhmobfb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fdimcluz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2swpdwdor.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mxrhckgq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ptqilqjg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tqpdyysx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2aypsmbxc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kthkmjps.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ujbcbpjt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2izmezgxo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtzztuyp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vykberpy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mjwwcmer.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vxjoeffr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xjejibib.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2baielkbw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2idsghqlv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2frognbgr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yjtggupq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2gkaokrrb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2nmkgrlxb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2woikmwek.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2romapscg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mvmmcuai.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2stoclqag.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2swadzjmh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2itvnxzui.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zzbaizjt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ecmvojsj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hplwgmau.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ncbfrppp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wrbnyjom.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rlhkhill.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wozwnumr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2iglnhtpi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qpctdstg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ueazxvzq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2diugvpoj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ucqthazi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2elzgkmzm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pyzkahmj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2onreolir.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2rkapvsxq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yqbnnqgv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zpwnjmsa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tqhvrdxb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cqtkwvcx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nswvwfgg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2unjeeenq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bqsaktvg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vewhyhaz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qkelnblf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xtqusnbi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2lvsybnrb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qiwhnfwo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rtaswqia.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fyuaauog.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2snmzyhyz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2eyraeiuy.html


<!-- 参考信息 -->