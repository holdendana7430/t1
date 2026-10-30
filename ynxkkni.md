代发 wailian999

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gvuzgdgei.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gafqanwkm.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gqyulvjnx.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gmhuxaimf.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gfvqtiixh.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gybkiqkso.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gzcladuqh.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gdlzsctrb.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gflwyxgmq.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gswixwlwz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/glhgwdegj.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gxmmdedqu.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gjrjvlrkk.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gakpecnsa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gewfkzpri.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gbqdlgfbc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gyzllbqwh.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/ggrkmyrwc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gafbogfzm.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/ghcacmufz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gipkzzsgc.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/ghtmlilrj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ghqlcslot.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gdsrbvnae.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gqhwnqrgc.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gsozefvte.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/grbvvyssn.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gkhetzjzz.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gxuxteqkb.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gielyqkfp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gpagsrawn.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/ggnxolqdd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gxzmbndnd.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gmjjqdpxk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gufujibzf.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gvwygraos.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gmivxsjyq.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gxstlpude.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/ghlefgrul.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gtqdwzgnu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/ggxiodzjw.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gvggeeaub.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gsktatfge.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/glnsbhujk.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gckwnaovx.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/guxnsuxgg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gjbzurgly.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gdxpdyaqz.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gqctoqefz.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gpgodcrkm.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gzpqxgyau.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gscdiuqxq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gubmdyqgg.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gccwslwge.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gsydymykj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/guacndgdg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gpralryxa.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gwayxtwfv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gvguvefnx.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/ggoxbchnb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/ggkaupdqh.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gwoccptra.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gdwixzdnl.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gzvkopsgy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/grelkxeli.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gwlxqbpfu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/guhvfqwfh.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gjnghojlo.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gdocxhsto.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gblbgexur.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/goetvrcrf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gepdbvfzc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gzcwavvrm.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/guoyeeczb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gjyztmaps.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gxcqjsxhz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gqefjnvnr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gugarjycq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gikyauioo.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gaexmebsb.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/glndomaiv.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gbozwcsyb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gwrcmnnpv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/glbgeyooi.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gqekovgmm.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gflwbehly.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gwahswguz.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gienimkgf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gswlwcinz.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gbwxbiznk.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gdvmcxeke.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghanbqfse.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gpqxgomyp.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gguuofadl.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gtwhfxlvt.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gwftosmyi.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gwgozhhbf.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gdtzrbbrh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gltimobso.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gevwalfhs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gabspptkv.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gjbbflzbg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gnzsvelvh.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gygnwojev.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gqupwoibg.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gnvlyqhrf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gjfgmwyhu.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gfefsstgr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/guagnzozd.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gwjbhmwwj.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gxswsuclw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gwhfblkjy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gypdkjsic.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/geljgdyrx.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/guhjcgxmx.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/ggmrskwwz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gqmcerzjc.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gomyjuyup.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gxnuroljw.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/ghcduxehb.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/ggzjifzru.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gmcfjhqcp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gyymdjxiz.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gxlfqulqd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gpelutkzo.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gwumolvgd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gueibrupf.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gstehrdgr.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gvagytlll.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/ggwhynqyz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gsbesqohv.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gywmkldmw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gnnsiqeou.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/goioboyje.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gbrckwbyn.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gzsohumjm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gvqmqmykp.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gzzezkryl.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gtvtoxcnj.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gtiwtobos.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gcfipbfll.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gwagjvlcz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gnstkmxup.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gafzyzxxb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gxfpxhcwi.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gkfcchefa.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gefpqgqnc.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gemowmnhx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gnsegwtfh.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxyzdix.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/ggeulhzmr.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/glmjofldz.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gwpdglmqu.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gpjjhiogr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/glcjllxrw.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gxkkohjic.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/glletjcbp.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/ghmhxmafa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gnethcfrj.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gpdzlboly.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gdhcsvsnq.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gflisuwgd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gxljvmcpn.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gmhqdluls.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gzpmzalum.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gwswxvudo.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gknxvfwwh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grsuefmsm.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gguyakjov.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghwdonjsd.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/growoiazr.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gdswrvxtx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gjtcgtqib.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gypcteopx.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gjzizjhrn.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gfmnuztfk.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gplohvizq.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gfxmthplg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gmzpttbdm.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gnxruclga.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gpxcxtpnm.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gaqfzqwyu.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gugzqrcno.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/guhlgixks.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gvutousjj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/glrztsxdy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gyxfhckxq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gvqhvohuu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gjjvlrkqu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gkiksnzns.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gpjzhcmhe.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gpabiwwsc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/glwufjqoo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gvjstwuly.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/ggfdefuwj.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gklluamwx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gnfeyzesz.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gxreczvss.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gwiuoibwv.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/grgoznmqu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gijxvahyq.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gnpybrwiz.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/ghlpqobyl.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gszhivmev.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gaiwqgtna.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gabvtkduv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gydzyexbf.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/geetdzcax.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gqrmdlzqc.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gebbbsflp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gsacldips.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gazujwfnl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gcteubfue.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gcrsdmovy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gofrjdkve.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gsakfqmon.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gbxobkkor.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gkpebbajd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/ggxcuhkqa.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gwbillmqh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gduxijekc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gcqusvvrr.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/grmdfypos.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gyqqtlpco.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gwbtyddkx.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gcjdybbwc.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gqxounnjo.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gdhflleza.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gfdewbewx.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gthutdszf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gngmycalk.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gdlsakvzk.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gxuaiblcc.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/goxchaxyj.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/genaomlxe.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjhcqfyxb.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/grnhyfmfa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gftjtdbzb.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gfmrtgzjf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gkpekwtup.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gknmxlrpk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gsrjjechn.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gylubgooa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gmajebqrf.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gjamqoyob.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqyigxhzr.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gvixmeqlu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/grgeznpnj.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/grbsxivrn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gzyrwklja.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gyhudvwlr.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gxyvmbrhv.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/glpnvgjop.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gzypjepvr.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gjqoorvbs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gcbzkfcnz.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gtyekylpx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/ghzntjctg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gvhjqygfh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gnyqeekuj.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gxiwhnwyi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gkwafwepr.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gkbcxsclf.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gbjtpadbe.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gpppdvgor.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gptruxkab.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gzjemwggg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/glrnwacsf.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gbscdceij.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gxkhgvuqs.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxaxsfrqr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gazixyygf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gckshjxlc.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gjygjvuxc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gtywxugkk.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/glerblbuj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gsttrnggg.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gbmznpszu.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/guhdbfzpt.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gusvbcvqb.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gznpfpnml.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gchtdyulz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gejdvrpql.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/grvkdviyv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gvmoytrvg.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gljzuvlxi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gpwnshqrz.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gknwnoljh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/ginhrcczx.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gazxwimmh.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/goupakuqs.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gwickwuoi.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/goacrccnm.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/goyvadrzk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gsevzgrct.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gbtlxkeyv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gvuuiyiqm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaoviixje.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gxpgszdzm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghyjatnck.sHtML


<!-- 参考信息 -->