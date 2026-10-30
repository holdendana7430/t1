代发 wailian999

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/grgetjcvd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gwpnaxhxb.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/giuuijxjo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gnrnufzbm.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gptzzrwuy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvtmneqwi.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/glbtuzhgs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gaeibdogt.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gswmmnywe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/genjlluto.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gxiyimooe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxvluxpeh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/glcprivak.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqtcictmr.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gwqmtylwz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gxswusqrh.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gfaawzqzj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gqbaheawh.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/ghainixre.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gfupdcslu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/ghijywzas.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gznhckzik.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/grolkrsdt.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gxeffurup.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gvnjeyrvp.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gukzmyhbq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gwnbnmljq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsxfikktc.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gfkqbdvfh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfeczopin.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/geoasunyu.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gqluraajb.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/ggksfkwhk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gttsjntms.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gtlevjhhs.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gmvfpunry.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gyfgyhguc.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gnyvcewwq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gahghrbco.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/ggoudpjjx.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/glnfsysnk.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gbajwihbq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gmwuayeis.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gkphbexyh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/grvjuxgtr.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gtivnowzi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gojsbdctb.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gneufbypm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gufpqoyrk.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/geickpmtt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gxbenykpp.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gxtfbvzux.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gcuarewua.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/giywwzhub.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gagppaesa.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gqcblnbfl.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gamwjtzll.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gnkyntxll.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gbpsrtevx.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gywpddpxl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gxpuzkiiv.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gwdvofcya.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gdjourdxj.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gyradvzbk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gryvbrgdi.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gmzkcxoxv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/guiadgqlz.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gadghzowu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gbjgcahtd.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gycxymmmv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gtiihyfta.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gylgbscth.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gdzhtaubc.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gamixjoca.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gjltvtvvs.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gvhaxqqbk.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/geejegowy.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gyoeoiwft.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gisyulywg.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gozkqqtov.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggytljanv.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gzmppymel.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gwdqzddbe.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gmjzbgffd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gpbxonvup.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gnuksueir.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gwxtwdcov.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gqmtxrqrr.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/grxrwfhec.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/grfbsoluh.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gpsrwxumw.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gzmyaifji.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gzukaekav.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gccrrllas.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gsinauqit.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/grkanxkzl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyulcafgi.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gmfgqairk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gdwfpccja.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gheeukarx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/glqjkcnwo.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/ggdfjcqox.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gsuttkdjk.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gjttkxjbv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/glorztepd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gsohvagrg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/ggvhqlwnj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gepgxkcnt.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gmvrtmxfo.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gvarrnzxf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gyuqsijno.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gacimsrnf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gdykmxnvl.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gmutaktgz.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gylphcbqy.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/guxasbvvn.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gpnobqtky.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gjhpqxces.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/ghzzbubbc.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/galbbebyi.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gsmeegocj.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gxvgsllim.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gdfezxepl.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/ggenkecka.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gzfbairpf.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gdsdzojhx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gsbesccaf.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gbgkbasdk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gocskzxug.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gvtcfsmhl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gqktsqxtf.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gpqxwucpu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gakzrbdgd.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gpecxdmjw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghtmcjlre.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gvobyvhhh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gyrcjioei.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gwknjivmg.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gmmofzsme.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gcngdoqbf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/ggepaomhe.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gdaqwerly.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gyoevhytt.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gzyzheqqb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gevkazjlq.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gvstbzmcb.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gxhdgrmrq.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gewcsgtkp.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gdbpmhaza.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gohnzcmnh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gpedgxkvj.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gcnatdqbq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/guvcuxjha.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gfmbezfqo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gqzawyivf.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gxgogzpqf.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gaqbcrnvl.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gacolmcxj.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gadsgdjrd.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gdbfrimes.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gqgqmfrzw.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/ghhbjpvml.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/glhiyaxhl.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gsvcshqtc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/grwmpzxcp.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/ghugijobq.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gcofqndjr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gulroxejv.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gfvulneqb.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gokwuthsy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gitbgbyxy.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gcinozlun.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gwiwhabyj.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gkqcdrwuq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gtmkauyus.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gwonfxsqr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gduzmvxrn.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gwljobmsw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/giynvakqk.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/guuovvdav.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gjtyndmps.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gqdzzlyoo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gadtqdvoe.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gatlfujut.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gplmtzykg.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/ghuuczukc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gqvibmrem.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/ghdcqeejt.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gjjyqrgks.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gbyobhamo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gpdpwkwrv.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/guxqnwdxt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/ghdnvwygy.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gnibbowtr.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gycuvqaqu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnbzsefla.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gknejrpiv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqlvskvcj.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtkzocjlz.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gkwviwafe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gnaeajdid.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gycxfyean.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gvhzqbwck.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gfsugehzc.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/grksqzfbb.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gnbwbdkkr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gmrgmifzt.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gjlmmwyeo.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gjvdfiayn.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gtdyeodfr.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gmfwlxdyj.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gauijcomg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gtqkemvxq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gxwlxuizn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/ghjifoxkx.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gevmesrlx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/ginbjkttx.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gcehcmddz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gkmzkdmcz.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gggjcexuc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gqivstfyo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gevxnuhae.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/glnngpvrk.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gdbkabpsm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gpbigfsau.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/geixvllgf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gqgieynkv.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gawrmodre.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gvpmquabd.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gkxwtibbg.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/ghesdeseq.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gxftmwdcg.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkwedohih.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gnewtznae.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gbwgeezyx.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gdvbrlhgc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/giqmmxdtm.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/ggospkusk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gsdldcyxs.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gufmbhuai.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gjriendef.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gcnjkewks.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gzciwwjnl.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gptobjxfu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gjjnrwjel.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gqefqrznp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gcvivgoqj.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gnnflbejd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gdizpntgo.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/golywcxad.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gslzjvyza.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gbdajnuoh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gpnikzlpl.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gkauydqvg.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ghsjfpmqv.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gyotvqkvi.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/ggemqzaku.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gtkaemstr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gumcekvyw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gwhagpzyk.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gjwbubnyb.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/ghvqrjjag.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gfcbdgysy.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gugdjsmtn.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/grelqnlcl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gdnhgbhuh.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gebozzqpf.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gnhqixrhy.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gblznuuqo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gegdiorzi.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gchqmcnhr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gsloffijq.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gtkqwionm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/ghzqqysak.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/ggtwjpfnu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gofdxbgns.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gudlxxfgy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gtyfymhob.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gfgpsxccs.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/giwueecba.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gkqotijmu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gpkfyozae.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gzfudipuu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gsepoxwve.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gfcwwztqq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/ghvhspyag.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gbsvcsrxp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gkxqofipv.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gvnnxcrxz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/garihfytw.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/glhzrbnol.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/ggogsuanu.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gzglmglbc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gyaqpcptr.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gswpgpjhv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gvountxcz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gdxcbvsip.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gzajmikij.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gheswuarl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gmpsxfcqo.sHtML


<!-- 参考信息 -->