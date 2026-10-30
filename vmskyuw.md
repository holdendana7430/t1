代发 wailian999

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gjbhaamuy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/grqmcjdxf.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gbgtwimxe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpdenbovb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gwptzyjhf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqtvhnjbk.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gvogaqrht.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmqyssvc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gvffxsdzr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gigbfeysl.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gpgkxnbvd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gevtmvcge.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gvoxjxlmr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gwrxxhaag.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqodzbpod.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gczoygsem.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/giozzxtjj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gqrmjurtz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gstatkevx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glmfnelyp.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gdvkwaawd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gholyhsar.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gbangkktc.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gsrpshakd.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gvqigxppk.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gdedhmooi.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gluokexob.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gtbbninbp.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gddwbcbka.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcopgrptq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gtrcljckt.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gvaosamkq.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gkokztynz.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/guqbbdqov.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gbcwqagbm.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/giuittwzx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gewokydue.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gyzpsvhbl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gsyvkqkyp.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/grufjiilo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gpgenbpeo.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gbrdpwvyb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gngmalzhi.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/goscnxblv.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gnrndahct.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gcyehynft.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gysdlyzhk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gcgfonhmo.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gnyrhexfi.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gnoqqglmw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gqsbafrdr.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gonqjppie.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzysxcfsj.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gffxdekae.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gfortvojr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/geprvrfzv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/genwbolww.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/getigjelx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gdmkyrqlv.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gwxeccrrt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gmwsiqmgy.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/grnkhfspy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gsvymzpup.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/guomjdtwz.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gsggukxut.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gthbyjovt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gpmxhzajk.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/ggifrwroj.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/guwuuiwro.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gzyiuiflc.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gefqgyzjs.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gvjgexoop.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gjkgmxjnf.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gtiohvatf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gewjeolzu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gjlmubzfu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gumsudsen.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gxydtrohb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gefuyndyt.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/ggedxzfjk.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gfdhjvvsp.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gsqqvviiv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gaiwisxdi.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gdgloexrg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gazxvupvu.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gfcidffqi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gkzjuvfpk.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/ggibuwigr.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gkhsclmhq.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/ghsoeeoql.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcclaadmr.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gvaneloby.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/giuiqqwiq.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/goqdmwvzc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/ghntdsbbe.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gwzprpstt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gxjbisbaz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gkoehxwze.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gfttlzqrr.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/guuqafhus.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gcrptofvi.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/ghzqlzbtg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gybdvyefu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/guzfoojvd.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gnpgdbqba.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gvrrqiyjb.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gumvesgcf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gtxkbxjpr.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gispblcwi.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/goknzexju.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/ggmruuvtm.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gxyhrlevh.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gmwmasugl.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gpjoayapl.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gbptexxqp.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gbtjlckwg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/girccnbyo.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gstykkyaq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gzwsggkbg.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gmwosajzz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gulfnftrq.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gqxhpwino.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvsskqwcx.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gbndufwtl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gbwfqxhly.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gnfvstebh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/galmlhcsm.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gbiusdyla.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gksrfohfc.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gbcovgjal.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gjhziqxgz.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/glrwwsrhf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gnbxwmovn.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gfyijkiqz.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gernaanqs.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/grpxhqanx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gwrcyndsi.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gvdunsigd.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gsgxiebtb.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gvtjkgvoi.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gzntofeoh.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gzmgshbql.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gxegyxhoa.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gktqaqflz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gdzkwzuio.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gaijeawsp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gmqyrqffv.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/ggpbptawe.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gatnzwhdk.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gctkeeiam.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gucstfvnc.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gauobkcmg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gsiuypmrb.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gtjunwiry.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gjuvmygsd.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gkvogqtzf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gfyecxjcq.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gdseesnro.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gbmpdhjil.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gimujfpks.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gbskbabdi.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gzuhhbxpj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/grcbthpbs.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gdvuhhxzp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gomgzmlqu.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gtvpmwhlj.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gngrrzmgh.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gykqlzuem.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/ggavbqagy.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gwiqvekvm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/grjndfpsf.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gqotlptha.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gzwcmhjyg.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/grpykbddk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gfulbrams.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gmnuilqjq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gtezbuflg.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gdlqzwbiz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gnungxidu.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/girnqhsjs.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/grrvkbvdv.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gzguqvhvi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gwckhcdmy.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gqgwejhwr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gnjezrbqh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gvsyxtznc.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gujzvbczl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvewdmhcc.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gkdmfixew.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gugdtsyyr.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gquyitbvw.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gyolftxud.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gzoumeqsu.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gxscatfru.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gxcxvbdlx.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gsbzoyacl.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gdpbhuszz.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gaqoiulqf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gbjrbhgcp.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gtrqwajqa.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gwjopnqgb.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gronbzjie.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gzioazfhx.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gjlcuzihi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gzvlotucb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/guozjqsok.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gujgrktio.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/ghbflmrom.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/ggvaumsid.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gfxqhwhhy.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gmfffhppt.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gpinpcdme.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gkjxlgvsh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gykogyuhd.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gwziqrbai.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/glejbmlsh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gozvbdzbz.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gpnsfsywt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gxlpeemit.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gndxauyjz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gxidtvxhh.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gidukdndt.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gdseyvohv.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gykrtyzst.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/geortzxhq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gtjpbakux.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gdbvevqmy.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gvzfaffvw.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gxxpawiun.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gaolbejwm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gankzkuuh.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gibgqrlaf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gsmfcueow.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gvqdgbmnv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gflnmniwn.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gbepeysxx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gzfzsvinz.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gfznwdlrc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gqdwxbvlc.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gllutuwqu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gzdltdcqf.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gyvebrgbs.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gptwoixeg.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gyoxpmrdi.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gnbrqyrzq.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gjnfsokqc.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpnfhlyzt.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gemzuwiaw.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/grynpjmrj.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/ggtzhwtga.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gxczqzhrz.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gdejcifeu.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gahasmqrd.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gqynleuej.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/geoohqxfk.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gergubmjs.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gkqgqzwrx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gkgvnzvhe.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gonixqdlo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gsheupfuq.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gbcsgdrdr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gjuqhjsfz.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gxhlgydfa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gqqfhtfwn.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gxkendyri.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gyacbmboj.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gmppryczx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gttwevfzs.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gsmxcsxrv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gmglmzevu.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gkvsdlavv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gplmlhhiq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gbrzodcif.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gkfbtrlot.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gjmebewet.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gzkznyroz.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gwqyxtgjb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gpcsirlyj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gtxrotakk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gfxoolzqk.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gpljfjfdd.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gdqnvsqqm.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gpuywkirs.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gtuslghlk.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gvyvyfigl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gujskgqir.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gprjhyrmo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gipwpjkqt.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gzpsbtzlw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/grqowvykd.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gyjtmeuuf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gzrbdgvuw.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/goqcagjkw.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gxaqsrrkc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gmawpjwqu.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gxmdgapds.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gjmcmvrcy.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gbbagovjr.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gwioonygb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gevelozxo.sHtML


<!-- 参考信息 -->