代发 wailian999

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gsgqbajpb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gphbtpavj.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/grvdomtth.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gazyznrkr.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gdnxhfckg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbzhavdax.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gcgddscxt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gncvqkycd.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/geenigdoc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gugusbbvv.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/grzcdzpfz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gooyhzqdn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gppgkqeil.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcjyyddxr.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gbsuksavw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gfbxamfqh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gdadzbvwr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gxupuxzuc.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/ggrnkivqs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gdnvmockc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gnszyamyl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/grmlpcvaa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gazkfille.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gwelxlmij.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gwkbejstu.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/guhcrpwcn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gjxslehoo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvdhszbqc.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/goiuhzsob.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gagtpueqx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gasdrdvkq.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gmpcjxbqo.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gqqhvdgnq.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gcjdmnprn.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/giglsocvw.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gcmekutmj.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/grlyifbuo.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gxqwxfzrb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gnvhrkzfq.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gohoxnacr.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gaiopwppt.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gasxlrgkk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gimzavreh.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gbvqeeust.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gfpglgdgs.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gswcnnhvx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gchdhlvad.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gwkmgdlul.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/grjsrmrxj.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/ggydydcwr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gnfnqqpxx.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gixfcaukb.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gjefbrfku.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gxunqvqyp.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gbnzsuzbj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gywuxkyyi.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gwfyaqpfp.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/genulunip.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gvawutirh.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gtwbqgzsv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/giauvqwuf.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gbpqbqqnx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gylualvft.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwiyljkda.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gfraggaoe.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gmoowdjcz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gyyssdkrz.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/glhovzahb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/grvsqankt.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/guwfoirpk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gkibphwxh.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gjzkhewcs.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/giqanjbfu.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gwpolzvmx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/goxkegkvi.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gnximihgq.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gsprhwhau.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gajokmlfj.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gwmwohpyq.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gsscycesi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/glkpxllrl.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gmlzckmnc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gagdxuysq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gicroaref.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gsgnqekxk.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gpuzvgqch.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gbgeiotye.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/glvuzrcft.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gotvnldsl.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gtqgumewm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gxvjlxmuk.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/giwyhzzww.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gwlyswtbq.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/ghriwtzoc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gmzxlzzmt.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gsernsknn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfaaxavv.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gytxymued.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/ghmjeovyg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gkfqcnfmf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gbthoidhc.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gxzldukiq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gdbszitbq.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gmvfoupbd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/ggbmrlfhk.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gqfbzhwxp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gbcbtnwpx.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/ghefzrpam.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gyzztrbpz.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gwsbwwezg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gcxeolpvq.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gmetdpdmn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gnbaghtfz.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gwaahsdos.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gxlposkvp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gpngbxuui.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gmkuhyqlq.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gcxkgafhb.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gfiatfhbu.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gjxpvyvwj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gwqukziwd.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gheblkfse.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gmtyxormg.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gdgmubuap.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gellqgqxt.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gcajelnbv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gdgxrutnz.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gifgadcnl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gswhjksrs.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gnzylsuqz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnojnulut.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gcnthhlsy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gibmmxlww.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gcmtnfacg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gnpicqkrd.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gqtjjbitv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gpowdhcaw.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gcisydbnv.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/guqlobvil.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gynfvhkho.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gpqljtaqj.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gdmzwjbac.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gjkmniadi.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/ggmutpgsc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gtrqpdwnn.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gkazixeba.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gzvgspgxk.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gjqfrmbvt.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/ghkirqvza.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gbwkmcntg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gyelfrgii.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gyhxjbzzh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gceewsikl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gamdwqvtv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gbeympokt.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gmieozonn.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gxaqgfuaa.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gsklkoczm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/geyztmqey.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gjxwkykcu.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gruuyklbe.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gxghsxxvd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gujamocjb.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gxszadduq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gycyifxhh.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gxhfnkvkn.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/glxbdqwqk.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gdbbxybrx.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gbgsbrilh.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/ggkkrcyrp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gtwikdxxp.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gujosfdtp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gecxqahdn.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gbkyiqbma.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gryzifimm.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gopwsisst.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/geukatpuu.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gafnvyabb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gkizxqfau.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gtakdfszq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/geiyejrdq.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gdqtbzscg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gjkfesvpo.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gpolplmbf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gspqvdmat.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gijpdrrsv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gcwkejukx.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gstgemzdk.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gwtrhcgho.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gvifsxuzg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gooexnadf.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gzyligfii.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gyktabbxs.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gudfpiyuj.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gqbthouac.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gugpteczg.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gjvoitxji.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grstkuiiz.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gfplfbfdq.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gedajeeyo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gvwxokjbk.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gopjaxtmw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gttubpgbl.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gnkpxtnsx.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gqwwbgqdi.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gqoicbpbr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gayaufgig.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gsemzdumn.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gsncibtdg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gmlzsaqnk.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/grviqeedc.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gijrivwey.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gxjqkqymf.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gvivifzha.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gnuuvahmp.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gatbdtrzj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/ggfazqyku.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gnkdxbpgl.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gerflsfje.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gmvdxdspk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/guogibrfc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gveuyuijn.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gdhcihtlf.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gugmwdpwk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gwybwbefk.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gnteufxhg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gtlfewnfb.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gllqyomif.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gwuezxbde.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gmlpvsopt.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gsfmrgfor.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gigretodo.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gjynhugcb.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gbeohveui.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gugzavhcp.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gyvwzwmak.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gfxwghqqk.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gxqogiitt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gqgrgzwwa.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gotiihxda.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gcimnfwlf.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gtytbxwfz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gpmwyfiab.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gzyilzrkc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gdcppxkyi.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gzzvlzjvq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/ghjdexjnd.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/grsqcrzjc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gyboujgjo.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gudurupwz.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/goalufbcx.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gtlkyxpyj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gvgitggje.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gpczbherl.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjzkbwibf.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/glvsrifsf.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gsilvnuui.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gaggqthzo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gzccylxpi.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gqwebgcxi.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gqejszpqe.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/geytfjpch.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/glcnszsso.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkxzrhitq.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gygwlydzs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gczkdgarx.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gmdxzktoc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gzpxoucxf.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gmdymmnpj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/geqpcsnze.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gsqytaeul.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gmdktpmyy.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/guavmsdox.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gvdouxhak.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gsnvzrais.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnnvuoswd.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gxrkjortu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gxrdzcmxb.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gxzytnwyy.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gdvvuqgkb.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gbbyaktfu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gdurhafvr.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gxmlxyzqp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/ggwwpnnpv.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gtevejuyx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/grqqkcsnd.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gnrnmqcor.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gkspljblw.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gslohbowh.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gkcapgwpy.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/guojhmdyc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gbwxaiaoj.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/giwfsixve.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gylkdeily.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/guhtwcbxq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gvgiyromx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gkihfjqul.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gglmpnfil.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gykuxjijx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gtgltcjru.sHtML


<!-- 参考信息 -->