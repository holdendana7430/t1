代发 wailian999

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gbwckftok.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gwwoziihy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gaetulhxw.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gvfjuqnhr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gmdbwphmd.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gzvaicoxl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gfzkwgxlz.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gncxtlcde.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gsawfgiss.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gaxyqkryc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/ghqsrnifs.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gywkzvsdk.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gdsgwmmbu.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/ghgopsohm.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gjvjwscit.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gwjypmkol.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gaqqycchz.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gaijklddw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gywlprsma.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gzlnmafjt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gsacrdhlp.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gdwlfdjrd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gveeioauf.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gxuelpxcb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqfeamosx.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gwgiuhoay.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gqqnronnm.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gstdnwwwj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gqcniwvze.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/ggqeywfvu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gvsrxikou.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gezvblhkc.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gkqnnrlzs.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gyzcdylki.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggagsefin.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gkatoaorw.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/grfmzxknn.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/glbyhtngx.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gfstylbcf.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gnuqzhfax.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/guykobgpt.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gpjdbddzy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/guwidnyfv.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gfokppvyx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gyjocqpjf.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gikqzlxyc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gfqpcbywi.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/ghwbwglkl.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gkvqcaysg.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gjppwvzqw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gejzerqpi.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gqwnqyanc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gcapipdln.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/goazqnavx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gfpmukphi.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gvoflpukb.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gwbhxpoqz.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gzoacenkh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gzqtlvuum.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gqpovntaf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gaucffaxu.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gscwqqcqm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/ghwsjphdh.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/ggccatchy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gtrhjynkk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gjbcxnqpz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gwwrtebbg.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gavjwfjdq.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gsnknuhyj.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/ghcdhbxfj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gmzaogmch.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gatiutvrc.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gmgpkvbvn.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gpalqidzw.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gejbceznz.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gynwifyhm.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gsudfziig.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/ggsakbyqw.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gepmijmkg.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gcyhmxvvr.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gfyrqhbyq.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gfnmxyyoq.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gxhxpuogt.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/geptsspnv.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gkuffbmuy.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gjwmfrkgi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gklvzjpfp.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gkbkdcpmd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/golcnfypz.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gxkurlytd.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gfgszjkym.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gyplwomes.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gnzdqeulp.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gshtqvuhw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnrsdlpxi.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gqyjjdrxx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gxiprwbyr.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gefhvbcuw.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gconnopgp.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gqqahtwrl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gbflqecgg.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gcymisvex.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gwhiovnqf.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gifbmoohx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gkwnypaza.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gpdxnlfxe.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/glsenieot.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/glcohfwwh.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gazwowyoc.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/glzryocis.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gqpfnhkfa.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gwpicjloo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gqmigiumd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gchsleyus.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gdoojkbag.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gsqfasnmm.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gaaibcbhb.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gohbzvxsk.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gdwsixxbo.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gpodkvntt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gikzqesok.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gflfokxkk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gcjckklyp.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gyaguezfr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/glrkimnrs.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gcwugfbiv.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gthwbkfmc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/guxqbkeiw.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gdekdbfys.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gayrlqzip.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/ggxdglhbx.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gxmbxbvnz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gyjnkyikd.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gsyrblthk.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gkuoisqez.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gowqgqvri.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gjmuxxvug.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/giipbijdr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/ggcrqdsve.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/glfzzmmej.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/grdrbindk.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gvidmmjpc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gvbtzzjgq.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gbocshghx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gqxgykbfd.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gwzgjcyjr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gftepysts.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gaxfiaiol.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gmwqxovcu.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gyhkzcbww.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gzdusrgbz.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/ganfdfjqt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gnrhpkerz.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gixpmmttk.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gumukywaw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdxdmizxb.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gownkedfr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvffyfqvk.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gsxooljfl.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gwuyqfews.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/givlxtxir.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gxuzzcfpq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/giaxwquqc.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gwyprejqi.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gkqyaheag.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/grgbtmlkw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gyglfhcvz.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/glbvmgcro.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gicbglexj.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gwekbpnjv.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gpcnkzfjk.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/ggornjhmx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gpmlwlacd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gdoymohwb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gozffgfmi.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gmppbwple.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gworrlbax.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gpflrbaav.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gyalnsshg.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/glqzzzgmn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/ghkklqfah.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gssetfapi.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gtfcixyno.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/giehbcnpr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gzzkmkfoc.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/glqzzsmpf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/grhiqazog.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gbfhoaomw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gpidpiylw.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gtxbwxncr.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gsonljxgj.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gqmjxivtg.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/glugqxlyi.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gvetezhou.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/godhwhvpm.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gidzrnxcz.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gamnsbclo.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gevlptmzd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ggttsgarp.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gcoxlacys.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gjjdjknjm.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gzuwdoyzu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gcafejfrf.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gwpshlphe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gegrornni.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gephwdgib.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gwvknwuyl.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gruzfppxz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/giugzpbdz.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gflzguqog.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gnxrxwbhy.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gflsodrkf.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gucvtgxmt.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gpjqktuwq.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfolrsbbl.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gxagavxyu.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gtirdekji.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gmatxdrtk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gexfsrlpw.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gyjcgsloj.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gocpulaib.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gcrbowloa.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gvbylxwxf.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gigknpbhz.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gpsyvuxrt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/ggqraslwr.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/ggbciwkzf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gwksnnarc.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gbqrczzuf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gydhjbfsu.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/ghxdeszfd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gnxaplxxw.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gwzbfybxi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gbhxwdjpx.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gfzgxbnxc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gzbwlitkh.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gsbwshajr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gjteqoomo.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/glxxkqrko.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/giaebifxj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gulmfistw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gzlwvxyyb.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gmagefnlw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gywlunhnc.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/grnpyefpm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gcxkrpazm.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gmlrjrwoq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/ggoruwdun.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/grxpfmqfc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gqninsuun.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gqxxtukti.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gvnlodzyf.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/glnuvsoeg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/glqbydtpr.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gtwshllht.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gvsadsmow.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gsjshlotz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gezlqljrr.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gzylqlrvr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gppfpjpek.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gfbpqorlp.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gcvbkcusc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gqkrqnary.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/geqpigbgc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gxbbteehk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/grterytue.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/giypfxfuq.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gwjfmhwfm.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/ghdfrsxlq.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gsuthxwae.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/giyxicdma.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gtznvtigb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gtiqbdzgf.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/grrlvkalv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gxiciwpfy.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gcwjsgrma.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/guktwwpwp.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gplxmnvfm.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gprrjgxgg.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gqltdugtu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gihzxzrso.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gperikvah.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gpuigouiy.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gatwipdvz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/grgskladu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnbrcwseu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gtfjlklww.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmgjuxbsk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbumuahgp.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ggxrijvxq.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gxaytpmyf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gszccnezk.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gdwiotdjq.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gqrpyfslt.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gqyjmrztz.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/grgsbjdho.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gamrkfhri.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gxhfriebz.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gcdkoirtg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gybziedce.sHtML


<!-- 参考信息 -->