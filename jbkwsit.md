代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gxllzzcek.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gmymoykdf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvyetjebh.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gcmqdirmo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gxnzxurjp.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gnceeuolc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gopzdyqtf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/galfctpid.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/giecslxok.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqoodclmr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gowjhxwyo.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gqxfnnqdg.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gzcmnozot.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/ghiommxki.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gecpjnolg.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/grossmbjw.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gxpwtgerp.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/ggiosspmz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gvqavmhbc.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gpubvrgzo.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gonllcxgz.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/glfbiaazi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gsngrihsi.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/glmmcreax.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/giqrjewyi.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gdtwlzcpu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gecuslqlc.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/ghikoedff.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gfgiczrbs.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gmkueiznz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gdtjzedoc.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gvmbkutas.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/grvhvkrhr.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gouncqedt.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gwwxhxaqh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/grrgaekrg.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gjkavxkrq.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gmvlnslou.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gnwvzubpx.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gwklfpvoz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxnyfsqvc.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gvvkmcazh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gkmhrfdjw.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gpqtvuomq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/glurwblmi.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gznynolng.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/ghevcxrbm.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gbxncrpwe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gurfaigmk.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gqfibjbdd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gbmtctpki.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gouvoggai.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gkcqflgxg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gugwumgvc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gfumofazf.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gcmqrpapm.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/grxmykrkt.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gvekvwxqr.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gspzbgtbe.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gxjasxylg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gkyxxvyrm.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gjpzwkrsj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gxohbskyv.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gomirhavl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gyfktwnus.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/goodhkjtk.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gjrfnuojl.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gnghotnce.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gtgoigvru.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gvwsnxgrx.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gvjtvryhu.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gushbbbhq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gsxooyqhi.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gjbswxvxg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/godaxdocb.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/grcknanmo.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gyipdxrut.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gcwccrutw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gdzebdczu.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gutnzdruw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gxadwhyrq.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gxqugwtcd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/guwudzhqe.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gflhgslco.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/ghmrmuzof.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gybrlvmih.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/guhneaqur.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gmkzdixgl.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/glkrjhhwb.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gozqqkgvd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gfslekpzr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gpbugyngl.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/ggwjxktww.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gtffzhnqb.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gtovquzum.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gvjdbbigf.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gooflnliw.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/ggajppldb.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gtakkxdrv.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gewonqnal.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/grvxcmdps.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gpetywpmr.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gxjbupjlj.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gyxgdiitx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gwnuzujvi.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gxcifyhsc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gcnnvjrte.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/grxxmcypp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqnirkivx.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/genyxagpa.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gnmvpjvwz.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gqdbznzye.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gvquziqcw.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gihqiscgy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/geeqlgubq.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/grogjpajt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gfdyiaiit.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gdrdgyweo.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gjuhvmkuf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gbvrugzai.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gcdtmorif.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/glamffjih.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/grfkssosv.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gjodmtdtr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gqecvvtpc.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gskgngcmv.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gbgfyalqv.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gtzahqnly.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gjnzylbwc.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gqzxhxzan.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gmogzfwjb.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gfjcdexnm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gkqlthxuf.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gpbomjaxa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gvkdvpaft.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gobnfvbjk.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gbdjiccsm.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/ggjzlrkcc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gltwrnygl.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gzdefmmce.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gfggacpvd.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gyfnzjywk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gkagazngg.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/glytvrysu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gouivblcz.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/ggqskakoj.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/ghtxwjdsb.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gbppzaqsu.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gkmiuvkyh.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gegycbzcq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gfhdtfsot.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gcvzeeros.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gdxoxzzzv.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gjzjxmuie.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/guqthxqhq.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/geabydlwk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gjqzvhmik.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gksbtvggd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gldhqxoiq.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gzbavezur.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gfujnlsif.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gccagqwxb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/ghpblweup.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gvnnxpewo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gnfrjhtil.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gvngyldlg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gjzsmrqid.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gwwxghfzo.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/grpuetxwu.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gxpvglqkj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gzieongqu.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gfbxyvlyv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/grpewnusj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gjnwjltfp.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gdbuixkhw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmfnrvbee.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gfseaypjj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grscxbopq.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gdqimfxrs.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gmdfrtbkk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gvdkorqyo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/guzyhqwya.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gnnoeveeo.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gseitlgwl.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/giuvfwtbh.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/grnscexqv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gzgcmfajq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gryxhsntq.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gnksqgtqn.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/ggrgxeobx.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gtkdebcmb.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gkrudmtkg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gblaztqqx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gytmyplqj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gvhsimabe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/grvmxtzel.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gifqegvcj.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gmxowescv.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gydqxjnxv.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvnjyxdiu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gbemvmbvs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gfpltektq.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gbjjqwxkv.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gdukjpfcp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gsgbpoqim.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gxlxheske.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/grgucjfjx.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gbqpqfpbz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/glwaebrep.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gthlvplde.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gjkjkxouo.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gmsxpgpsw.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gmlcafuri.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gmewdjgtq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gmkshxikx.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gsbteehis.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gtwywnucm.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gxbnxytkd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gtgldsiaz.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gicdytzwk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gcerlxxbm.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gzrkvekku.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gyoskvqmq.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gjlvjjlxx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gjkeknkks.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gjsrrnrdq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gxsfrlpzh.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gghizgxgv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gdjtfqthn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gpxkgtgsn.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gcjutugux.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gyvvaerzi.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gggjxfgiu.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gdyrozjvw.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxhrborne.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gojiccbjv.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gdonxzkka.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gfztoalzx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/garmzocdn.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gmkyszqan.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gngmydhlr.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gmrksslxn.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gzzdaceud.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gofzxuhtg.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/ghmsxcvgk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gegyvcrxw.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gjrueeiwu.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/ggddesoga.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gzdbwgshf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gfhsazkdm.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gmlknoewe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gnbrhsfqp.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gjtixtqni.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gukyhhnrw.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gvvedekrf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gdqkmxnmn.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gxrfoqqwo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/geaybkifj.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gkbrspdox.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gkkxbgwwy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/genejyvvg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gpxvjgzlu.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gizxrjgdu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/ghrfirftn.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gwpgupgod.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gtrdgrquj.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gwhjqyaid.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gwzcyhrli.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gnimayqvg.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/glqyrqquy.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gzllusblk.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gqemidwzx.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gaihpvxmj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gtraeykse.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gjfgzdjsj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gxjbbaazn.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gxgwaflsd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/ghwrfricy.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/ghqvdkauh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/grhiyqioo.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gwahxrvgx.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/grsgykwds.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gprpbfdvj.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gdgjexyrc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gydnqvegs.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gycyofouc.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gtpkfoiuf.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gdbcdxykx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gupxigapc.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gmhppxdne.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/grfneeweh.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gqswgtmdm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gqesvwqfu.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/glruebdkb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/ghsfguexb.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gryzrzdwr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gwevrouwe.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gmlihbcsh.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gjrotxwsx.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/guyknsnsg.sHtML


<!-- 参考信息 -->