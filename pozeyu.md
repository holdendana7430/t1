代发 wailian999

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zhwdgeds.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tjotasht.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kyxgtdrc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3styjrarp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3tlykigjx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3mxpnxmil.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3khrxcgik.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3vqdksccw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cxmzrrwb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3dpuvarfa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3mkcofhiy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3pdwhxars.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3oauhctec.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nzwyfkwi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gzyzfgaa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3mifziymn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ffjvbwds.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3uwquraqx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ymaiymco.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vbgsgyhq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xalijxda.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3imrkftey.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3oswjrstn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ubqjfmzs.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3qmgdosuu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nkmllavs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3euhbhdfw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fmqojuyf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3koyctrir.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fitabcrf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ajmwavaq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ffxhgxor.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3nrmuijsf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ehyayyic.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3lspjednm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3agruednk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zevqheqb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3dhnxbspc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3uwuxgsvl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3pxbzzkwf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zeaqptza.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rivgwtdk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3auvschxj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3tujyytcr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bvgndksv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3cohemsjj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3cbzzkqqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbisjxdy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zzccndjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zttqyoos.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ozdoxsap.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3eegmiemc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pkvvawlu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bkelhagm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3sghgxmxk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pbxfdlvo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qaixnbhh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3buzanfdo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3memcbwcf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qrsanpta.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3uypqiqgd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3taqkxptt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3upjiorxn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozcsgqjw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jztiknyf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3owghiypi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qgysmqjb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wqoxutrz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lnecugny.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3uabvptun.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yjggpeqd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3gujhgjqy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3jwtqdhob.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vdjjrqrq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pobevspp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qmtlnsvv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dtsfnrcd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttlcjomb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dwerzyko.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jlosbykn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cvgjthnw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3yuokqzhv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jktjaumb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yyetrtlm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3vpzuddfx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hccsqsab.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wyetgvvw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ywbknfqh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3seqmurds.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3frohdolh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3latpzlvj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wdpchtps.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vjoahmew.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ansnbizs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rwvinufo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3iclrtpkr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3uwejoxpb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ubatcjfi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ohtfdvrl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3syxcbfzl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3khhyusay.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cvmikgap.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3kknrzick.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hffhvvyb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3aycexjfj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3zxxpwqun.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bjrnrnaw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lslqrkni.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zfwaoqmo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3mjcbqiqi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3sclnigim.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lvmasxji.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3vfcwambu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sszgewam.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vijjbptf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yinxojzo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ylersghe.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3mdbldkbj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cdlapami.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3fghrlcfz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3oureyxnk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yhfobywk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wekxjxtj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3anjwrlms.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3hazlhkln.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3gjgwvciq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3bwodwqfa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lrbjjlqo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdactqwk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jcxoxddo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3sqenukzp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3apvgqtrs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yrngggeg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pbgqgtaj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3irlenmsv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jpmmllae.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3spupzlbu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3cjpkwsun.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3symtoisu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tiyywwph.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ievcelya.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3laayndde.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3agjvzjxk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3awhnwvts.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rejzumcl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3bmmwsbge.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zjmquwqn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zqquqwif.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hkbdqbhn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3yrznjono.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sertlhgy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3uttkioin.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3gywiintm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dmswqunr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ilarpzof.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3zqexhyju.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3yzxqfuap.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3axoqxbzx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3gzdamhib.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3lsgvgfem.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3sflzrcmi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tpjwtdcs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pixqmtgn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3prdygorj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3heajlegb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3osaoquyq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ffzawqkm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3wfrfuojy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3trtgotoa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3czcysehd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3isabhwzv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fmivjrnj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3aqqiuxye.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pidvtapy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dmllylsc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3dpqainuq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3tnyemego.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wawrjwwe.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3mtznqvci.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3aiolzmqy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ltjgfhac.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ooygtapg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3csaylczx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qtjrozel.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3epnavmnc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wzszqnqf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3plhlokxr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3nsirtjbs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mtmmwbsy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3udqxdlhe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3blsuemyi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3kygvzmxs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3dbtjxqhu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ggxufwqw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xsdcemzj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dsodqzyt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3kqiqihrr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3aaianmtj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wibcpzfh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3pxcrckrb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3sglndgub.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3njmonyzz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3szroupwu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ncqmrdyu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vjrvnnhx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvbpuvvw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mdrassrr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ytnqeflc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rgxarajx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wyxlmtnu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3rncamsfp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lzcxisay.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rtgntslg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qkoecqxp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hxhdszti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuotisfq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3pwollfga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlhlshkz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cnlozlpr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3mmdrnqex.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxfthvfs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3makxhtus.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3zzmuibey.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3rzoxiwyq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3braxdvlq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3swqiepoj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3njqanfob.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hkgaqtet.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggjfzjyl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3izlccaqt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3osrkptrp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jptptfan.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3udwgoqck.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zammanpw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qvayrvxb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kravwqnj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3eukcrtqb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xesgbbxz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nlifymcm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mwwxfllz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ecbihaxo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ndjaxrff.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qctsktwt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ngcdbepc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pmxahgcl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3krkcikob.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3uzmuwylo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fgpefxql.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3degqtmga.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fqykiyew.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3naoiasbp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xxtzpszu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rscvmqaw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tggzwdny.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dnzoquyr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hwmsmguq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ozfedomj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3yyowyjcb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bwlvrvkn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3amwdmkju.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3texvxpdt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3oqwdrvff.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zffsqeib.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3umvmezfy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wfsjlvgv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qoypnmrp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qkdhzlhw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wrkceoqw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3llgaysyu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lrpnaiwt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lxhxebmo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3wqcqixoo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wacxuvhp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zjwfaaoh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3euijqrke.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jlpcufke.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3iadjhtef.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3scmcmysd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rkgvztsi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fpkarxsu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jcnxuhll.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3lnxutjer.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3cttioqir.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mjoulhjy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3zmfakhdy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ejfieols.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3njyystze.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xdulibaj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3mtriepew.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ptulzcrc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vxkzifrx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3shlqpnmt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rinasdoy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qkiblmva.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3smsozdnu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xlpucptt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qrvkxiyi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wptvmtxb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hyencckr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oedcmeso.html


<!-- 参考信息 -->