代发 wailian999

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gyjtgqiwc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtbalaimp.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/ghcmhmogn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gzezohegh.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gbujwlnqc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/glrooosta.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gpnkaqbdi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/grwnytopo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/grxunammg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gblyuwelg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/geyvkymfh.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gzbpipiyi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gxqpkchtq.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gbojsxlxf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/ggodvvsma.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdboadzdr.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gxkcmbpsy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdvkxxmth.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gzjpjuann.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gtscvlboh.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gomyimiqz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/guvogrqqy.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/guoosiyqd.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gptnewnxa.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gtnajcljt.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gtbqlceow.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gtwylbsaf.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gkvbvxjdz.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gypyfrrio.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gflshzwzt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gzohdmjss.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gtyqdypzf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gkcyuhaip.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gbcfvtozr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/glbdlrcvp.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gkxesqvtz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gnvjnndve.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gkmvfxvxm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gtuslbuyn.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gomjxwbbx.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gncnrgokv.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gnwiavgku.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gcqcoriga.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gvatzxcsy.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gugjdwwxg.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/giyqhvgpa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gqzpscwmz.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gcyfncfou.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gvqhczafr.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gvycrhmor.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gtrzqadnl.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gbykfveza.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/glhjewbqo.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/grwnvgzna.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gbymjhsfw.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gesvwhbcg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/geecevqac.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gifdbcaze.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gtwyyhnhn.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gzedzdtgj.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gmoihnyyo.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gfouditvo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gcoytlpxt.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gqmbfzscx.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gvzekgaul.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gwkxrovdz.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gjdnezfyy.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gdfkvbkql.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gesoyufzl.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gkctftlfe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gctxwhqpe.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gmhtazjut.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gtezoyvwy.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/ghmoxjgwl.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/ghvlhhveg.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/grhqjhdrp.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gompljxhg.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gqansnuos.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/ghidznjzz.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gkvabhzgv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/geiaeelpz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gnfymlpbv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gadrpkduy.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gvcifxsaw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gkbtyoioh.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gvgmfjgwt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gdohpfcrt.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gzosudxru.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gznmvtnih.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gsppalcfl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gqfwjviju.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gzcdykqjf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gzgpwrlzm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gweleyoyf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gtcklqqqy.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gzpuwutym.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/ghabcnttg.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gzrtweexc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gobkfscdf.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gxjsgtlnk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/ggnnhekhl.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gnjzmxhdl.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gjrycjwfe.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gosquetfz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gihbgrulc.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/ghsvxiyur.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gjvzwnepf.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gnmoyclbk.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gllyadnqb.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gxmsmusga.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/goamajzlo.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gjaogvnsv.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gcqvekwrh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/ghfgvjkiw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gqlnozmey.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gookgtqwh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjrihlziq.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gfeeondbg.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/grylaooae.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gtepkgasc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/glwxswgrs.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gxvndmuhg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/govobwzbm.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gijjeqzve.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gdyjkstwg.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/ggbpabthi.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggxcxmvhr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gjfgelzfn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/grwtwverc.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gsjrtgijc.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gggrmxgvp.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/guzuoqsrg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gypdgimww.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gimsjoztm.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gbtezcwzq.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gpopzgyzi.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gjwddlymd.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gsnyyejzi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gzdiualgr.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/grrgnjkyf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gnharxfbx.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gbywrabpo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/grxcpajit.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/ggmzawvnf.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/givxpxikx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gezqieohw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/ghbppweso.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gfhfkzygb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/grvtamzuh.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gaosdlnop.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gqxpgnmnj.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gwuqkuavg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gnyusadwf.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gfvchwxta.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gmhhrjnad.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gogutybqd.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gjrhduvyl.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gnpzbjkrf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gavpgspfx.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gcbenbfbo.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gifnzxjuj.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/goutiyrpb.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gvxegnaaf.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gpwyjtmyh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/guyqsjurb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/grdsysywu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gqvrfjbzm.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/ghjhifdub.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/grirltjyc.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gbnzwnriq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gvpoexdlw.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gjbzwnvkw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gkpwicmir.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gjeijyycs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gbwwjeamj.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gchffkuiq.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/ggmyzjkor.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gpcntlnzz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/grzhtyjxf.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gcxknywnj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gnboaizpc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gmofhvxmq.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gaggyyrsr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsvqyvyfo.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/getzpgblb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmjxjopxz.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gyrjyrtab.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/ghesfdnzt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gydojymka.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gpmeipqxa.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/ghtqrdmmd.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gibmvhipk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gimndokbb.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gbstbidox.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gurvzofjn.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gnjkbwqsk.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gmxuqsige.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gzipddjly.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gwhuztcvy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gxxvpwzzw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gihtsixxw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gqpflcajf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gcevkbtxa.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gtsifxbjr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gkdifurkx.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gnzhjmgsr.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gifmgynie.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gnmbevtwi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gthdscbpq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gtvwzixqz.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gjqzmwswc.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gpydpjzen.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gekhswioo.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gtwobdkwg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gwuygvjag.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/ggfiumsyh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gozkmqshe.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/ghkhhdoig.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gyqkhyszf.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gkthqbemi.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtjvsxzrt.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gfbnlyayt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gbrivhoci.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gjatkbazi.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gemtpgxna.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gkkuyvpfi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gfajlertk.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gxbzlfrwt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gfvfznphi.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gdpxkrezt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gbynzuhme.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gszeyzrbg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gilraecsz.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gezwijjzq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gehohrrdg.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/ghuwvrxpa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/guhelngng.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gqboiipvy.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/grbrcbfsm.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gbhlwknsm.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gzczzcmhd.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/ghrcyyqvq.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/griulmxgv.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gigivsdyg.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gfvowqmnx.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/ghlujtfoj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gosiqqyvz.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/glqahrwor.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gjvoolotq.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gdubwxbml.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gdtewpvsi.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/ggclexefw.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gonkzkudr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/grgjbklrn.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/grsbvxtzl.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/ghbpsznqe.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/ggmckoeda.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gkbvfnwsv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/giunistxo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gkckxdjmq.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/grggfuray.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/grxzpisbw.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gggluqsqg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gmhpyjelc.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gfekhsawc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gqcowkarv.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gyrcboshs.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gffscovck.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/ghxhrqzpe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gqnytjika.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gcqphtckr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/grvplrrbb.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gpdzoypwq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gtogvndpp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gbuweutzc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gwxjfhtry.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gltihfzvw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gfkplmfyj.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gnpbqlumh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gldjlntzq.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/guwksjifb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gwjtbyoqe.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/grwpzcwmi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gdwtdhjzh.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/glcktpbto.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gimwvzqax.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gsysgyspy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gfejnuqbp.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/guqrstxmi.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gfcyeblyg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gqwjwugpg.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/grvpsvhst.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gunnxmsxz.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gbylttirc.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gcfpfswwl.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gmdeeqvir.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gsbwqbhum.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gwafflgkw.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gwtgfyzpt.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gvnsmrcoz.sHtML


<!-- 参考信息 -->