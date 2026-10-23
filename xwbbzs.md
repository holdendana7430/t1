代发 wailian999

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgevttnn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3emchbgue.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nomvirom.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qwiipfad.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rmmxbzrk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3smjthjhz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bkykbaiv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dbydxdlc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3uklkwwzu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3pzphqjck.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3mpebqchp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3fdnzhvbs.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pmupvgxf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3snwzbcbc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xmpmykxj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3sochccoq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mzfwqwoo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bdrrrmnj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iovdyuwq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wgiveiwh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3umymwepi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ajhfywzh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hfnoknbg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3frwwqoew.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3pomccgzc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iquanccr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3mzhnxtvr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3kezubtqy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3yzlfstmw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3kbcvquiq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ojqnccuf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tuezjxsc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3sqitkjdx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qppmuikq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ssioetnq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xfsatatk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3pugcqogp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mvtbmqnv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3iijerwng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djezdfdn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3znacbgzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdlwczpz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3tljdioda.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3omxqvkjq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3lkzhwtox.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3jxiqepva.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hoharipj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zmkfxdaj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qkqydskt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ixxetyso.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jjaogscp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jrtgfbus.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3lnqatsqf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dsxutkiy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eghizysj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rhicdlol.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ucbpsmcq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jupbndlp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qfbbaakx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3etdhsllr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zzeoewbw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mrkeebzx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iglwmcja.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3aoimunwn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3knxrmymr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3zdzmyxju.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3yyfzruhj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yhjoezgl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3reywohfo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jleayhsd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3quvoaljn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fgyfudif.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qfgkufqi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ucjvpjid.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lcanfhfv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ppbsnbvf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3giahhjgm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ppimveix.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3legrhaad.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ppzactjg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vbtozjti.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3fbdpldbf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ccxfzsjp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dwslmsqt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xtgpkvip.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3nifqmlhn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bqzetyab.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rngwpspo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3nchwheci.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fnydrwmz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3waccxbip.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kzfgbfme.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dpvzlnut.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3opiikxss.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vmeigahu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3nqmneele.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3lwrngjmy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3wfuugsdl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3vvrfljpn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3iknynyff.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ruuiwamr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vynlbbsc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cmfvyilt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lfsvjqgs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ifjugrxk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3isyfikah.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mpugknxg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ixvkaaix.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lgjxagqs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3olpvownb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsjumese.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ymvimmpm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wvxowptt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wtzpsxfn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fzvnjycm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fwvukuqx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3baukejvd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ivxzullt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3izscigfe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tgibkshq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rokjhzdy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vupvxvzu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3abqlkjnn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wqsxtcgv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3apfcjgjp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jfzqxrur.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rgrlhrff.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3digmaola.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uytygbfh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3tbzviupr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gkkbhdjo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3fttgrmzg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pjogyiuv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jktblnys.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3pkulbiib.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qysxofji.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3aydxavad.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3njxofirj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dduifolw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3glrlsxyj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ujnqwhxm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3lezfzlxc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mlnfzabo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bzvueoex.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3oddqvjci.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qnyjginm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3clyhkryd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3kmgihbhd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3mlgpcspi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cxkdzyox.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zoqfjzlz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3okgvnhtb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mqvazrwe.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ccbwsnhp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wrbbnsoe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3wztkdjan.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cnkgazah.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uafjmsdl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3psmkkqee.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3uxjuskog.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3bewghtrs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pamvnkym.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3tbymyabc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sneofxpd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3btmrinsp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wyndefrm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ikixyhfa.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zrmdwngd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3hfpxamcp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbvnhajl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3tlheeoqh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3dclzzaxl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3tdsgdudv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3pgvvyohk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rxkynhvc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qqtzjgic.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3irydojlz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vwakdfam.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3sbnfyxwn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3fnzstzal.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ikpijfss.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jblastvy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3dczmxwzs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gmgibqmy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qzvwldih.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hgbvyomc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tnaiijhr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tkinyrit.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3dkiltann.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zdzcysbz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mebpfxgi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nsabfkea.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tvklemuz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tezpqcml.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qsyiplpq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jjqazzpm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3fqwfstgn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkxtvuzy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ykzzxklw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ffeilqhf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qwhwtwol.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3oqmtdhhr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bzdkoach.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3cqwbrndw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3tmghhcwt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jxingkkg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dvmsqpjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxqrkcaq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3tydmjgzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yixcublj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oyazjixu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jhuokvnf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3okzowbss.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ooyshwzh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3kzquwqqi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dhazpkfj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cotslxfq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3iccitkzd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3eqqbegyj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tlxdwgrv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xocjokkp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nuzahqht.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3nvweekte.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3eifnrebb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lnroeerw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gfgyulfb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tgihmdxi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hivhcwix.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wkmsverc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qgqmxowa.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mpwtnepx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3esxsbycb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rsiejkbu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rsoofjyt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hjuscakl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3onzlhdjg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3idjprzof.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vwgyktgx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3odivkgqe.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rqwejwjp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jmalhckp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qazfckgj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ldljrdiq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ivuliklh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zbniarti.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ndptjsjm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lbimqvul.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zzieligx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ppscueym.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fzwowqwv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jwptsyao.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3cwmyhfac.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tewhhhjz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ymaovaln.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xutekzwf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3sfjlppuk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3woxpyloo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nabllogm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pwvkstdl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ovdswvdt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3thcbhwzg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nzbteoxf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3alfihgrf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vfqockch.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rqxrlbbl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vrlgzsrn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rblwixmr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xoxztrjn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hmpfiady.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ejsqjcxu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3xkvmxugf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3svsevyle.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vwostyzx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3chhtbomd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zlnugzav.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nnpnfqui.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fuxewzaq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzpwyeyp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zrumfrep.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3erqtqbkt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wbonazpt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sljozgay.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3pwhnktlf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bppqbgzu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tcpjshja.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ovakcyny.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3riumnjfh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rrzhnnuv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ydwmebja.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vcfytvof.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ehvwdgoo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3scnwspir.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qpcquiqm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3piduvnum.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wgjeoehy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3fbalgylg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3htioviue.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3tjhksyjf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pzrwogqb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pgtepvxn.html


<!-- 参考信息 -->