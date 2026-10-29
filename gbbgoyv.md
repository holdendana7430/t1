代发 wailian999

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gdujrolpg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/grisdenbl.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/grgeogkjn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzpsgjrtb.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/ggvzlsdlg.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmofqcpdp.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gqaqbxbjo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gwmvruwzr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gukgmzcxe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gckbafqad.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gxmqhflln.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gldvwlblq.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gqudnsxqg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gkslaytup.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkugmiosc.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gwalcwglv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gpjimtzxq.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gxethdoug.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gqxtdxvws.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbdaeryuo.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gtrptxqvi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsixrqgqf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gdrbbmkgs.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gszbevgrd.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gznxrqtii.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gxpftwlix.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/ghpuwzljx.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gbwuuiuln.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/ggxkrbalu.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gpcpgqkny.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gliirbrjt.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gjfawteep.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gffonttpt.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbjdxovgu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gsoeqnksr.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gglwoqizw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/githpnyju.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gfykzxkdl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gyyayrsjb.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/giaxzaoqq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gdualvrnf.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gwtcmfvts.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gcgylotkd.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/grwlvkkyd.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gdstlkuvo.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gdrvabxum.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/glsfmudld.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gntifhslu.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/grtqbrkpj.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gybbxoiym.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/geuduiljy.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gbejyacks.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gyceqjuiv.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gdetwelam.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzfcogzyy.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gzvmdngro.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gxswfshvk.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/glmaojchk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/ggfgsaclx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gpjsarpyb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gbokjomlu.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gpryenfjz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gdpfjumup.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gykvtkcbe.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/ggutlzzbl.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gyovseelx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gamwheadk.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/grtitismj.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gylxameds.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gmranihcu.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gzrndeqyr.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gckcsuekp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gidvvmeou.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gpyzubcur.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gzlzgpexr.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/ghcafrctd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gwgkdncsx.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gudredwpo.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gjdrxghjb.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gamarftce.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gbueaapcx.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gxujhvtww.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/guetjbfqn.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gvvsndfob.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/goegfjapy.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gznktmxnb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gdihjyhei.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gijmuryke.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gwcqcbuwv.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gxqzcaoke.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gcgtvicpu.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gtntccdgz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gvktapbjw.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gyynlfqtc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gvabeqjhx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gvlrgdewb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gzfsvrjre.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gskilfiue.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/ggdxogqua.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gryljxgck.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdcwjsnv.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gmogtdkfs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gacrclvkp.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/grkbbhpzz.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gddhgpkwi.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gjmvembhg.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/ghirvjtcx.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gseecckxe.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gqbsqfcsw.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gatebpypo.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gjozkgakt.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gehjcwspy.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gregvptxu.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gowiigzsm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/ghwgdhwod.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gfkglnqeq.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gevghptho.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gbkhzzetz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/grhlrujdk.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gttubpips.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gaiyakzxr.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gzclcjjbi.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gamuakohh.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gcoyefxmi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gfakptzgw.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/ghfuekdxi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjietmuru.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gulbcttfo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gylvizgpk.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gwwrfhrvy.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gxfokroih.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gjawtewid.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gmbgljhpl.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gqwyxhcvr.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gucdvnppp.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gxlgziilg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gupklymyu.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gcfpixsnw.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gainntzpz.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gpipxsirk.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gqtlpuiut.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/grzdgdwdt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gtxledsjv.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gswuwqrur.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gmtnubcqp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gnmgshxnq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gpjwniqwt.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gxezwyunu.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gqlcnggpe.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gtfurjdvr.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gmannbwpe.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gyonnlmxw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gvvigcgmn.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gekmalcln.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gfzxagitp.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gsqztctax.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gpzgvmdzd.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gvhqzafkn.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/ghggyjxbp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/goeiofvrx.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gdtyurlkb.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/ggmowkinn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gzvyjedlk.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gvbtwottv.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/ghbnzlogn.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gruppofbv.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/glzonnhgs.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gdldfhpcw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/ggdnormyj.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gprixmgrq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/ggobvmiow.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gblcuijvu.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gmhcwdbch.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gdblwsudo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gmtafxlcl.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ggdvdjnnq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gcghjjfbs.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gmekxcdbx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gtgenwtfs.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gslfviaed.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gdzmhfsrc.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gfpgukhlr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gatywfqhj.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gifttaiom.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/guohvfvkg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gbftibjwd.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gkqhlvrpk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzobyghua.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/greqqdudn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grmxpjich.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gxoyntyhs.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gupqohtfx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gfnzlclhg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gpouzysgd.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/goncetkpv.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gvzhafjtq.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/ggvagnpjt.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gxqigvjlw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gryfgudpm.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/grwvvzwnu.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gmytvbswp.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gdbjswmnh.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gurorhnnu.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/geglyzkkc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gaxnjlzza.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gftaofogu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gchlxarxs.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gduzabvho.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gjnrdmkwq.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gofdecjlo.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gywpejbtr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gvnpxvhaj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/grgsgezln.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gmrmhzubi.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gjgzhijzi.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gfkzybiea.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/ggmdcazzu.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gqcsqhhbh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/glegvajtj.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gdtqwoprf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/glbvmuysm.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gpevradsv.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/ghidwzgfo.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gvonmscwf.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gaiujcvvi.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gadarmsuv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/ghmnhobmo.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/ghryymgyd.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gejbjvbky.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gvewcmbws.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/guhjxpopv.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gkkvlbden.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gxbeocbnf.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gjhkpasre.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gklrrmfde.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gzfwtyplf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gqryrbtjf.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gokgprkxe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gfkutbklm.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gsxpjfjof.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gxdyfhfwd.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gwdhqlcgj.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gsuymthxu.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gcrdvknhw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gtnezeeuv.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gfjqorcea.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gekgonipy.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gtxzdpecx.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gwhudcdnz.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/ghjktpxlf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gpsivmpxj.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gvtqehrjo.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gfxbdtlcs.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gxjkwdbxc.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gmnmgxdxw.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwvfbwrbg.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gyocajmju.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gmacfnhic.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/grjvtrdfs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gebywysov.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/glklfeyie.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gyfobxziy.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gkmdlkaik.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gongicteh.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gpdltkhfb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gdsnvfcsd.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gzodqaebm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gckociwja.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gvzzonppw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gatltmxig.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/ghnlycnnb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gbhurhgff.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gxrkkhxgo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gxcoqrpmm.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/glutuxzmj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gfogxnodp.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gxeybshum.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gzukidwcm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gcrgbfotr.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gxuvstxzo.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/girvpiypl.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gmlpkagzn.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gpeiusgws.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/ghvgzqwnh.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gvqdkmfzn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/getxfxjsr.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gmjitznpr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gzzkupboy.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gccvulgyw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gslsseawa.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gdcmhvpvy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gdxilumll.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gcvgkpocp.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gvoenbkjx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gygzeqnof.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/ghlitjbub.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gpitireab.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/ggytfmksr.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gwjdlgqeg.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gjzjupror.sHtML


<!-- 参考信息 -->