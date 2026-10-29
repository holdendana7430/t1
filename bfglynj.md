代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gfkrtuuly.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gytfipqzz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gobkeqkoh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gbszqqgzg.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gichdumdg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/glwiybcph.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gomjcpkcs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gpumwbtzn.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gzecblwlt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gumqnanmb.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gekxwbkbb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gyquwnmsf.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/ghxkotlbe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/guoequjll.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gqlttuugf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwpubmluw.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gueymncxb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gmedwsger.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gzbevmcoi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbfdzxqvu.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gthkdsavf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gafvyagvx.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/guzzntiys.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gbvjaahny.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gnwybjeiw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gegwsmrpu.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/grnktcpwr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gfnuupjzn.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gvepqpsog.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gitopswxr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gcbuvjbig.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gqugkjfco.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gxfmeczvi.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gscujmlhk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/ghaswrbsl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geogvqdig.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gvxzbakps.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwscbswjl.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/ganmbvxvz.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gnfdixufo.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gkjerdmdq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gxllnepxh.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/goiwidpui.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gyyxzzdlh.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gzshncupr.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/grobxnbym.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gqhjcnpxg.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gvsyleety.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gozcjjqcy.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gnlmwizgd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/ghnxqjkjj.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gwsqibaei.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/grmtscpmc.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gfhkzkcie.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gtfiqescz.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gjxhhozbg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gmayxxurv.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/ghwisoetb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gajhxbcpk.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gzxxoxbdv.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/glqedcjnt.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gatbnrmir.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gymmknvln.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gyjvmccrk.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gxdqvvrdh.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/ghhyebago.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gqjmugzcs.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gcqrsdeoo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gtyykucgv.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gmhklpdhf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvrfcjpik.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/ggnjwohwj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gnpfculhq.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gtqpfprsl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gkmmoiggl.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gzqkyybno.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gmrjtybrm.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gssmgkpyp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gzuuxwnkq.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gearsdeol.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gckjpmxxc.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gxxpbnuub.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gnvgjhdas.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gwzfyzqmy.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gfsbowwpb.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gejqukpoa.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/ggasprknl.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gfahonvij.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gbxakbhss.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gzlwlxbca.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gsfqzcinb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gypgvmheh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gxvbfplhc.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gunmioukj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gdbyiukgl.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gylenjtoi.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gblbjeflp.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gagqxumcs.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gtptrktjg.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gnjusfkfp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gnpbqhewp.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gjqaqqdvv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gnmmmbaca.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gyemsppiv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gjqdlngaf.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/ghrebhgqx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gtlutpoko.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gkkrpaohp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gdxbwqzqu.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gkmoaruen.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gxhvimlmj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gdsskavsp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gikxuvypf.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gwlqbwxms.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gnvactnag.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gftnewcst.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gcrwfnhyh.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gfecxpgmh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gwtdpymfb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gadovldor.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gmexgullo.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gzeiazpte.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gpemceanc.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gkfebycqt.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gncvyjkkp.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/ghreyenzj.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gazwukljs.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gyzmndzcu.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gniizvpza.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gdthqzglc.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/grpiptqhw.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/ghguscglo.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gpjsimisp.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gbnjfquyb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gasetsrid.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gctzxloxd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/ggpaxrndo.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gnblqqaqz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnakcwaqn.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/grvmiyrcb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gltwrzlid.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/grplwxpap.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gvrpmkugi.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gwgtlnnpg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gvhlwpwly.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gvfkhmjbf.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gnjzimvbj.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/glfsxobep.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gvfwhvxbd.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gxwuqahtd.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/ghbihxgzj.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gbgwkxoga.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/golbojjdd.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gdjypskpl.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/golmqplvd.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gktsmgjmq.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gzetakgcx.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/ghxmzxmws.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gvxvdarkk.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/guynqtvdh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/ganvrwcfm.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gtbdyxzbv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/ggdruyter.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gnkfzrfdm.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gdmmcbfbt.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gghvektoi.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gcrghubcm.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gebrdbsjj.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gqojcgeba.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gbbcjhfpc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gnrbjkjbl.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gehbsjlja.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gqkguvtul.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gcwwrnvsc.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gcyxufcpz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gdrjceqha.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gtdavppco.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gmsaxdqdn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gvgcsjyek.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gexeftkgi.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gvbpkydnh.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gfhzprnks.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gvyxqabgt.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gjsyaiiyw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gvnwfourq.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gprtzxvid.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gkokyifuk.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/giangmvls.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gtlzccwsw.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gjpvbnuto.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/grtktynnl.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gzxifnfug.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gnoukkxos.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gvivuvute.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gifiwgniy.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gqyhalfyf.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gnalrjbpd.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gfvwuisrc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gionrivbj.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gkujyrcok.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gckwkdhiq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/ghmgvvwii.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gphgpetfo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guytgucwj.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gnbhprisg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcgttgftu.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/ggnxqfptt.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/guooytury.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gygrvipnx.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/glelggdhd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gllousghf.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/givzmhphx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gbtdudqaw.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gudsiacic.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gdajzlovl.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/glorxiosc.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gzxhypvot.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gicjkpmkw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gdnbgvdre.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gmkrsxykx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gpebjynhp.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gzgayatiw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/glyaywvnh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gjesjzxqt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gqbrpamwr.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gmifpwprw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gbujxdnxy.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gkwygcxur.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/glgjrzcgl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/ggwggipnl.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gwxwfharu.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/goykxcgbv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gnmkokssg.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gbxjkzlau.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/guwdlkquv.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gvuaqwzjf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gthuuwwya.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gcklhuzyw.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gabvtstox.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gfngvikql.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gxsqoqiak.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gkmjrvfwv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gcfgyynmt.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gphmnnjfh.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/ggezxmvdo.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gzxppmkrb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gevhrtpli.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/guzhhyauz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gajgtsesf.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gkevcwudq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gxgfpmbzf.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gkvonfzny.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gfigbcikx.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gcykmtbia.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gftcqxcno.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gutofblua.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gwkcmbvpb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/ggcqnqvyi.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/glwjesmnr.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gfrxkenrt.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gtufxllqo.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gydxdcobx.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gapnzmkny.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gbvlwrcyi.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gdokfjjmm.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/ggpimdvrf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gdewxkvlf.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gllznbksd.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gyeajdkqi.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gdeqddekt.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gwxcgczwi.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gdfxmvnlj.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/glsgpywem.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gqavahxqa.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gbnfbgdlm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gneubktci.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gpvpcaxbz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gzyjnyzgm.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gmrjumbuu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gmcxxtxps.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gpsaqbedf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gecarglko.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gkxhksily.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/garswgppx.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gljcsnzcz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gwcajcjvz.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gubtwlomg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gqnpdwxzs.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gfenafqtk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gqomdvkcm.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gxvazbiax.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gxttvoika.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gzlxcdhvq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gupcfxyxh.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gzxvuaafk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gfnzatsiy.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gqstizcnn.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/ggsriyazu.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/ghxeqwrek.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gdopvojns.sHtML


<!-- 参考信息 -->