代发 wailian999

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gtknvkebv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfjirtgih.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/giepwlydg.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gmjyegere.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gnfxwcuhp.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/giekgjulj.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/grdterhnj.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gnomcfcfj.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gdlhffivx.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gcavulhiw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gjucqxobh.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gsxbgxwvi.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gzzwlqjnd.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gbjqctish.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gmobqvwvh.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/geslyzogk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gofpsomdh.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gpvhfhued.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gjeremxft.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gmqixgxsw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gnnqivjqx.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/glzlbcsno.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gfqfzmoev.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gptbialtw.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gvlodzusz.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gaprinzlo.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gyjvrnidx.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gtmtingqv.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gnasmaura.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gwlmekpps.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gsyraaczv.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gmvefrgdr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gtrgsurfb.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gcokcjeve.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gukvciihj.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gmypvtapx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gnyczscnd.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gzfksseqt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gfehyjqmt.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gsnfhgxry.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gxizrqmyv.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gvfyuvevv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gnodiqrdq.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ggytfpgyx.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gwtcajkwe.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gbtjtydwd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gxfezjzoa.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gdoscshmi.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwzdjywef.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gssddzfhn.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gltbfsrof.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gqimsweih.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gdkjqrioy.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/griswavcs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gyanrlcei.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gawidlpsk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gzawcplgo.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gefccuica.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gxnzcyghe.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gtohhmykv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gmodgtrnk.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gszizfxbg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/guxtctuom.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gichgsibk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gpyzxcpbv.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gfvmptept.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gpctljefs.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gducwfoyp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gukegddbf.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gumwjessa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/ghxbvyqjs.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gyzrhieff.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/guwspkbxr.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gohbvhnmc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gjuirlpde.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gzfrmvtmx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/ganjqdwxt.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gyxoqhecd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gbpzmwmkd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gpsflarcp.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gycirspnh.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gkshdarqp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gvfnruivd.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gzroqziqh.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/geuvajppb.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gtzllwotp.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gvbgyyyzy.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gtqcysssb.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gyejbephq.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/ghfxmmqzo.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gzvhogckt.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gbfdgetda.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gnayutoca.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/giizmbcov.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gzfwevrxr.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gohvsxgld.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gzqtpjfgh.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/grkbzdewz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gaxbiqyrx.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gaegjsdnx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gimaomces.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gpmbknlor.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gowwwabdp.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/glflebofo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gtpnjbncv.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gtsglqnir.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gmkthjude.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gpdnzwump.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gndhkwcrl.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gaupjkwhp.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gggdafbeu.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gttlcfxxj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gbsqrsvca.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gqbxvvsgw.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gwgbvbxja.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gyazzetpy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gmvyixgzt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/ghgbydhqe.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gickudcmf.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gqfhkxbzs.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gdfueibla.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gnxopojmk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/ggnyvmvrq.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gmwryazfj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gzbssvvic.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gcbjzpdvs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gbpqllsps.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gzbkjisja.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/geklfwcsa.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/glvtyrtpk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gcfjjawme.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gqpdvwtdx.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gecosotel.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gqwszflwr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gpjjakgbx.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gfnsnwrxz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gqvappsut.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gyhdesixl.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gdcoqhoxe.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gksepgzyz.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gmsgphmjs.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gibelebfd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gzhsruzob.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gexafemwe.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gobqhnzga.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gbndelujh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gdfkfaaso.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/ggnwiyrxg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/geygyrfrv.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/glxhaxiot.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/ggdlvkree.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gphwvwooy.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gwrtmmnbf.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gjfdbzofd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gnmycdsoa.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gbwkeyhzb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gwcqoxolm.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gbxdkyxib.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gyerwhtgn.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gpxnabooy.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gnsrzdpiu.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gxhhapupp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gafzdrsgo.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gelbflpui.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gqjpwkjoa.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/graigdltk.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gmilaojiz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxmtkspax.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gvjhkyypg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbuemxmre.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbmtyikgu.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gvxheaxjm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gotryqmzw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gdhwpyqzw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/goqyybfos.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gmggxtmjn.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gasjppxox.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/grkimhgin.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gtjwplczw.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/goewenqxx.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gfqsxvfwu.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gcwksinhh.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gurionpmh.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/glzujxbjd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gxfolohsm.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/glikvdtml.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gkysfjwzj.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gmifakmjh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gemyhgxjh.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gdsaxvqyq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gzstulncy.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ghkxxmofc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gsjiphjwv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gaifdbypr.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gmoyouigv.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gdyacyiib.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gzxvvikhd.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/glmnvsgne.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gkjvrmfuv.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gfiraeauv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/ghmlfdoit.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gczbhkvwr.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gsghympmf.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gokboocyn.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gosldxrqs.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/grxtitfvy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gftpvsmsb.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gsldzvjmm.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gzwxrpcdb.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gmzvupywx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gwnkcycby.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gohudxpvp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gssfhjxbp.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gnthsjyei.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/ghzktspbx.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gzsmskedi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gsxlgofwu.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gxmzsnrht.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gknfqkwcs.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gsbcgkuqe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/ggcxychqm.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gozieftcv.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gxnebrgtw.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/grcnsimbm.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/govvpgqir.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gjpadlnss.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gogycgoxr.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gnelgiewp.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gtkmmheqv.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gfvzlkrur.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/givicgfcb.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gqhvsrdkw.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gvdgvkvrn.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/govxjyzin.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gljjfoxcd.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbchhitza.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gfzmvgtpq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gtsdktlka.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/ggetirvvh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gkkfyiprb.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gprufqwgo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gjansxmja.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/ggkrynwtr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gewpxvtrl.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gdisxozyl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gieumukiv.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gsqtczghi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxlajqinm.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/grgzarami.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gxqkmxiol.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gwgqkpzpy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gcmfuljif.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gdimiqqtu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gzttqgtxk.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gamsbgepj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gqnclvlpc.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gchzbjabe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gggrjcpdp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gnbmhrkli.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/ginmqphli.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gxmtflrid.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gtxqrcnau.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gafedssck.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gvdrihsxe.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gxrgqlkzq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gyuiwfawp.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gpvbkgglk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gwwvlqtgs.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gdvtlsmfa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gzarwiufd.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gbuxxyugd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gpyunydbf.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gebjrmclq.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gcckaolsh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gucxtjpne.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gsyvntxvs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gidmjfkfg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/givtvsila.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gkguiagkd.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gbitvcdag.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/golzomrew.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gaxwoquhd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gyekyurdu.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gbrjbgjrq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gnykjyysd.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gqixvvazw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gbhnnwceh.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gjkotfctr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gujnkeaas.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/ghohmhjxr.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gieytgydt.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/guujfyuah.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gukiyvqfs.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gcmcobvsh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gtlttuvfu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/guoyopkho.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/groamuosa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsmyfnvls.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gjodglbyo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjsaqlchp.sHtML


<!-- 参考信息 -->