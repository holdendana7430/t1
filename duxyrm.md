代发 wailian999

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3kacwgmwj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dstlzski.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vslojnzc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3qmdpkzcj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dcvhtlgv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ajeyqhqo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ehouwmep.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xrwuwspu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3lubsbvhb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ssxanxje.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pplwogwm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3msopylxh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oprhsofn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rgrrcjcz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3eqdfjswc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ggfxiexa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3enztqdrf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3unsxtbfc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wslwuptx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ygqwgbcz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3yrudqnic.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3kznroert.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3bntjuhsm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mvpoyjmu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tzvvfnbo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3lhuwroau.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pkgtltcp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3isebkafi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ilktdeqk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kkouxyke.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pdotvvqu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bxgvolam.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3fuersnut.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rlsfxsht.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pzykrlxg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ycvzzcxu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wwnhiqpy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ffrzloqz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3skujzyjc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jkxldzvw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3bauculcr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3anfzzrql.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tyouasoy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3xcxjobkw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3tyfolmwq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hppsgtwo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hcohjxph.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sqxptxro.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3jncsvbrs.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wacbkyof.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ipemkrtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycgvqznb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gpdtekgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjieovhq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xnjafnek.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3minnxnxe.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tvnzrhga.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3odfzstgt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hlcjjzme.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3tlbyxvzk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3aemhkjua.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lloiwzjg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bgledlnp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3sihorncz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zpiqkumg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ubvralko.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xnnrciyc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tzuhtskt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lknmgowl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bxxfbrar.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3szqbwrir.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fdcxocug.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fyjwlijg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gqdzenar.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3pyuoccxs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hjsegktl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wsgdkbii.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3sxdspang.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lwdzuhhk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yowivbmp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hvtgkkkt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ucrxniwo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3whhexqcm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hpedkkyf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xyvflaua.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3dmsfwarq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cfbjcsfl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pwooxhhf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tslnmzxc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vhdipnem.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gxkvoffq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3cqyqqsmv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vcsfflab.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hopumxhq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3txssepdo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ogktnyqa.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lvrxjfpe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3upstspqn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gujwpakh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pnydgjvd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ftvpcmnm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mybgflgk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lwyitkcl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kxqqrsbl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nylaozgs.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uwtnenca.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ebpjngxm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3vekcbtqt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xxgqcaoi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kviuagmw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3eloggrss.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bajijrah.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yxjygdiz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3tmilhzkh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fwlbxswj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqhvwewp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3foejhkls.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3swajfhlz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yxlrmyag.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bktrvige.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lzfwtunj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3eqjessfl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlrvtpgs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ocpgpeyv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3aelmtvzo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3adchugyo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dscovtfd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zznonmrh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ywtaefko.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dpksymgm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3deellbnq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qytwfiri.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ejxvpnsy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3koviauio.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3kixvwfsh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3akkzhgfr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gnrfbmkx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3kuydsmeo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fyvtllwv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3eurumvcg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ulyujucx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3sruujhta.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gmvnlqdw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ordzelfl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hjbzvqxe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3icqajpdr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3enlfznmi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ypmaxcen.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cmqaessy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3tyathwsr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3cdahgwyv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wkgjknut.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gxugngge.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dgygbhae.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rnxxyxfy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3cjbznujj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3nxyexxxs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ctszodup.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tmmxklsl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wxkzkgfs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hbojpwar.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3uaqjwjzx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vujaiuwk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xbarfhkc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ossmiofk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3czgxrfom.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pvssayzs.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3jbtoyrsr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3estgktas.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ujkvxetl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3klplilxw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qmhekzxk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cfhrwwyr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydpflwjd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wjgfknwv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3doavbjiu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3gmpytaew.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3lbrkopys.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zpvndzyq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zubfexcm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uqigpnvi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hrnraufn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vsrppidr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3oehhokne.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rfqjkiic.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bchbjdci.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3oledonpn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rtluvccn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ynqdxsjb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mpgbjinj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3cadknrcj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hwubkyuy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rgqzcopy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3hizikdmn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xrlnysny.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3svzwabdi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hdjfmdai.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3frtxfaqy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hoddzllr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kwcgyyew.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ghjoydee.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kbkqvpra.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mlylsfwc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ueutjakm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dyicyxvq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dgalbotz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3xjvtfulb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bsvpifzi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xkcnytyg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zzcedder.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3usvqgzex.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3sewvrygd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fckyewkg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gkmdqqmw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xrfwykdm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gzldqeaa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vnmebcqp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3cncsvtpz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3armmdijd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfwyncig.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iybfbdkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkzddyjd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cxmeybmm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3asnejnav.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3cmrimrjt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lstgqysb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3awslnuab.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cszuvyln.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3tjhsgzij.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3aglxefgr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3mdydxovz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xooxmymv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3nyrcwjql.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ojyitybm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3utkjxpli.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jafxkeaq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3pklpfrdg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ebfevwce.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3luejxtgr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hpieaeem.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3boskvikk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ikegrrnk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wzybeefr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwcartps.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3uqpmffgf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pjkzxbqj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3shlolvhe.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3yxtvindb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uakfjlxo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3thrycvac.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3pkahliys.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3uwzfflgr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wogktmvw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zpdylxll.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pwuwlfat.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fbpopkif.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3barqdoqo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ejibbqil.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3esaskvwn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cgzygonk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zrddcecf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dgzkxwgq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xtfllzwo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3urtanfik.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dpkotkkk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3uhkmbihf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3piednftt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yisluzba.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3acdwfjms.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xwuvbrkd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dxxlumlb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3udjlmxmf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ymgjaygu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3uhxomfgq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3frhzdvsn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kxtmwsvt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kowxutuu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vrckmzps.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sqqfmqdb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lsimugqb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3hiijnucr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ksoeatnv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kkbhfutf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3saomprqc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mlzouxwm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wzcnbzuy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qkmqhxlb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rqucclpa.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3vkivruty.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jluxzmvs.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fwbokxel.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3kawlfgan.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tizrjqei.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ldjutcno.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qavwdxtp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3tmhokely.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3btmrntfi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hsnttior.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uczaivpy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pixjsmro.html


<!-- 参考信息 -->