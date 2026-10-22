代发 wailian999

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2psxctmxs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rcfkvddz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lugkhion.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zrsoantv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2iertemms.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pvsmjgnu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ubmzhhqr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2uwvschuw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jgqfwnua.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2kzzrktkc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jbuveuxb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qdqjldzs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2nipduzjy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2buekkcdc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2xlqorxif.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2nrwgqjin.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vovuidxs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ccgbyiez.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ptmlyheg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qvmgwmed.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2buqnufec.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zliyyzia.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2laayuhks.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2fbcecgeq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2udmbfhqj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jmwnmvlp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2aqqqyhrt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lrziicfk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ijhcgzvz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qlmvbczr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ptouyjao.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2rcrxbzpk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2nphwzgdv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zjhuocui.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gudqhbfa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lxjrcuqu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gkmnkwuv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zonlkvah.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qhtpqmci.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fgwpsema.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pzcqktci.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nesxcdyi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bnkqtnfl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rkbyumij.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rjujihfx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2fuhxwvut.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2djgzmmeu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2pzviziqs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2lcetuscp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bdpoxrhp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ywwzumuh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xwkbagee.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fsikmwhz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tebwtzzs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2egdeffel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zlhdyfob.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2spqbylms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnfiinwp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lzjlxaku.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2nnnrgxtt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zoxrjhlf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2znurmssa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2drqchshv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2hgmigajk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2oinxqrlo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zcdwlcce.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zhjitthu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qeyurrhh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xdtcidqp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xzuotdck.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mehefbvf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwwflaav.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pruimfrg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2eqmeqjut.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ppacwhcr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vwsqvyfr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2apybcutd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2whtzdygh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xjabuvbr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hgkfyzvr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qbmxrwry.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lvxezybx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xshodtrz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pezibmet.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jxzawlmf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2iemtjwyc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hccgwrlc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pjuwcizt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ikhlysmn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mqgewnjg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qvvsejlq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gmvqwwbr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zpaikyyi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ezaywqzk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2haxagpyp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vocmndyy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jzzlzinn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2sbnhmdhm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2efmxfubq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zajrbamq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mhjejvaf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qbzgsdww.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bmqkkzte.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rayycpur.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2uhanapum.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2otmlhsli.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2izptpwbf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ajrirgbl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gbyztenr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ggjxssqa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gtfpmemv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2cajdutay.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqbgrdbk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2glybflsz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2tkwlhudl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nityjtsm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cuwzgzoq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kqzxwnwl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2utvizgir.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ilnriags.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2peexlqvz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xacbjyql.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2vibpkbqg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2lnzrcwvb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yisndybv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fiarrwgw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lycjarns.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2mfbgmseh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2gmyrmigi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ltiwmdju.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2uagugyqx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pyxddohn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ltythqse.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jfeddgrn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yilktiin.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fcwuholx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cpcoetxi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yzuvfidk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wzprywct.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2olxdgqip.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jyhtgzyy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2omhoqswf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hhhybcrv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2fmgwzcfw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lkbvxixe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2yfmouqiy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ywfyxaej.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2jiaajqnk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vyjoufjo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vuatbhbn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vvyqyvtv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2npetsjiu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2lpeaszsw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2oxxdpapp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zwlpawvg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qgjvwzqy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2olzbjyyy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2oxvrxrxw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kuygkddy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nkrwnvgz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tpkqbbap.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2pbxckbkt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bixfexhx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2hlgubfpm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cyogfmhq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gjelnrtw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2endoccbb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2sntcwwct.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2enowjgiz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucvzzeex.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2auxcpoll.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2basswfqa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wganyrys.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gfwldqxj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2bmzsxvtv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2jfipaklz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ubtuqfct.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jcfqawfq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nyeorqmb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ugbrfust.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uqhelfwb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nmdkuney.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vuzcffni.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2sxczcjdb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xkjynmkf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2yaezgnoz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2amqikpww.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jmtsiwhg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2dyalwddp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qmzmszzg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2njggostf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rfkwhmlt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bvspdoky.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2iniiiyto.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nbosobgc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vhhablvy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xeuuoakd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qwlihnpa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yfyufgpj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dbtljiqi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nqxhcqzg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vqhqmjjj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2uqsegcsg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vgxjdyqv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2iqgidhxj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pfrzglvo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hbozdeoy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2iennfssd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cxwsdpcy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2egomdcle.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zkmuzpel.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2mhsnhzsv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2diupwhoo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xicexhaa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2umewebqc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ezillsej.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2debtmnfe.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nfupjflf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ereormat.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jwafoevy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ncpemcqp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2begfbavz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ifmlfxcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkbivckh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hoohxloo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sklqigcu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qhbxtpau.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2afflhqfm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hylllljs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gtdnaadp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2pbcojvbd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mbxoalhp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ppofriwq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xjfhdvqx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2oyuwutrs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cspzlaxi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rwsrgdql.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ncrchngf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mcjbanul.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2opkhuqmm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ocisofhb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2cxcyeuzi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2enqiockw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qrhkzrte.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ndqqiteb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kzpumndy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2boesepgb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2taywkchz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rpxcmvsu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mkjoqdzm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ntwnytnb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqxegede.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wqukupyb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xczmhlfa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ghsvzkvi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ywlblbaa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2oblbvpdt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fxiqwtvr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xlwigpdk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2sgiilskz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2amlsaqql.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2viwdbxgp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2nprwiscw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xcgsbwyv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hhzxdkgg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xprisyzb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mwfwqxoh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2orveislu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2oyfdczwg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2hdpivgih.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2iczbkhal.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2alizarco.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kyisnsyz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ghwkshsd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dtjztqce.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2jfuagzfq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fpzfxblh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tdnvtplk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hivapgzj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2avivsxot.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2sqwfeznr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2axipjdml.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tijdvyrr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hpdhjbgo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2nyvgpcnn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2pupbdyfc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ikxoaowd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2qjlswoud.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xkdhvnig.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2najektil.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2iscqyzfl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ontopfkt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hnhvdkcm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2cihripxx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pelaionn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qehsadem.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2kmfqcown.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2opvvoier.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qaykbkqk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lrnfesuz.html


<!-- 参考信息 -->