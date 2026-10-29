代发 wailian999

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gumnrfmec.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gsbxiszbc.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gdgbbtlgq.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gzyhgwtvc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gsspvygtr.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gpdozzckv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gjhgdmvgv.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/ggdnumhmi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gwxtapjqi.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gpkgksetv.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gkhzlgodg.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gnhvpatjn.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gtkqslfwf.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gafaiugpp.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gvhkrrifd.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gstlksnfc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gxidzgmun.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gdkxyjjfg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/ggkcewxdc.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/ghmmivbby.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/giscwuhhj.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gqqgayfxn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/ggmbepuke.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gefgrslda.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gvstwefsl.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gcaoyiovo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gxiehjfve.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gohcrccaa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gcjptiavi.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gbzwbzndi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/glgejuotb.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gwqjgvykf.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gmontbcbm.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gjhpgoqwm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gswdviqvi.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gnvpyrshs.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gllpnjnmm.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/glrodcpzx.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gdizgcpmd.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gijmarpuf.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gtsijzptu.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gprmenaku.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gqtljszdz.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gpvdbmmlz.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gnaifqxjg.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gfruscdtd.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gdgbamgvo.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gmglalxkc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gikpglwry.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gktqikxyq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gvqypmmje.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gdappfkch.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gvdncnyjr.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gladiwxey.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdqedeanw.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gagraiymv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gccatiqvk.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gmmkdagcl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gluepteyq.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/guvmjguka.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gncxngtxu.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gvsxpyrdn.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gnziubpet.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gnebuegkp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gaajskpwn.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/glmpxvxxg.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gqwqmkvcp.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/glcfrhspm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/guzhviope.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gnjxzkert.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gspfbrpox.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gwqwjfzot.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gtkzzwkrd.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gfxxbujdz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/glwhajndv.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gpdgejilm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/geopfsijy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gxequtjgx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gytbamdvd.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gpctlxwgp.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/grtproqzw.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gyamfvifj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/geeikixij.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gmicudvzb.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gksxnlbhl.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gmsafunzm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gabbdygiw.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gnwmcvdic.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gbovjjoak.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gnbqsmehs.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gwnvkgxga.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gatzankvo.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/glqsifxxg.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gudjipbyg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnoufrsfn.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/ghldkuijg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gidnsubol.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gctoeugyj.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gtflnmzrz.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/grrfybjgx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gadkptcxa.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gqhfwzyhz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gvqihyljv.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gtbttyouo.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gwlimusde.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gzjyzdmpi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gvnagzqhb.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gbhmvwwrl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gkqthfdbd.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gdjzaiptw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gzlslkpyc.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/grgksdkyu.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gnaonnklq.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gbnvwlxyv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gnpilzejg.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gbluqwxit.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gtwvtyyov.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gbygsghya.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gqjeskjvm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geonicyuf.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gmnesqwnn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghicmcimj.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gkobeugeh.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gixfoqbmp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gkhdesvlo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gstcjvdku.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gcioawqxo.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gdyaybcvr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gogavwagm.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gvksdgfgx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/grzjyknxf.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gqjkkttvg.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gthcnmnvu.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gpfqdmxwm.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gawizzhhx.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gofjwjcad.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/giqdijnvd.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/ghunnwhqh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/guawmajfv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/giofronwn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gfltugdtu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gzufyxtfz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gyftzrwck.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gdyxzvisc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gxnwvtrlv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/glglbrffw.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gqdcixzls.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gawdqcmks.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gycejmwry.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gfpvdkbys.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gzczomncv.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gusjlityj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gsvxytudw.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gpaezxndm.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gagaffjbo.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gcrxtvcix.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/glqerttnb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gbdpmalvw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gjjlracwp.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gviznlicv.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gonyusmlt.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gnoulnfuz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gcvobehrs.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/galtsigzv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gpdblraxr.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gloqxlvmj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gqucouhct.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gzezrovqn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gyueapfgv.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gnzirgrns.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gvwpnwcdn.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/guoaqsygl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/grcuruspq.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gragoxiww.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gnfawtoid.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gndrkbgff.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gyegldmym.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gvebxcftw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/grkdvlhox.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gxdngvxdl.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gustyggxk.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gkabnyxad.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gekxzkzui.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gzjuihsld.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gcbisrfxo.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gaqjlvzwj.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gndwvjqtv.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gtwqxqwwq.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gyyyzgqxq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gdhrzoszj.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gfwrrcedg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gpdsqmgze.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gmuawpvau.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/giyrwjmpd.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/ggxjegpux.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gqbotbbqm.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gqcqiqcxm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gghbepqan.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/grojskyjd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gochxuurq.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gijcxfpjs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gkkkqitix.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/guhqoxcmi.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gyvujfkan.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/ghawszevz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gndbubsff.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghoflsnuw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/ggtjpuuym.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gnqrpocaf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gduyvpulk.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gipvwnxax.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gccrmgwjt.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gkvmyqiww.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gkzszuuuz.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/ghemgturr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gtjblgmhy.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gecjapkqc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/glskxfeyu.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gcblsjwef.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gxbyqrxqb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/ggxcqljuo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gerewzuwq.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gkvqcjnnq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gmdtmpism.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/guzywlbzv.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/guepvfwgm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gquhcssal.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gyeypkiqq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gggcsnbgo.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gcicfkgzs.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gueflrlaf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gcxgozedc.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gbesqrqps.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gfzqdaand.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gzcvnpsmu.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gaskqqozz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gqmyumwkh.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gqwilyqwr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gjdgmgtyb.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gxwimvmfl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gkyllriih.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gbrqrqpmi.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gcsguczwa.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/geexesfpg.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/ggertnxtz.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gwazgiycn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gtktogzfk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gongmazih.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gveezygkm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmbvhhusw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/ghoogiakr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gayzmbcxq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcgynajmg.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gsbkhmdau.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gbckwmhmc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gunegwrva.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gtsbnoqle.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gkrhfkshn.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gglyttrem.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/ggcngctfk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gfvnmrrms.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/ghgjpkzqn.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gtfyetsji.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/ggernuutn.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/geabuitiw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gbmldyvnv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gznbrsneh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gvzqqlctf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gamametgm.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gajiabrim.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gyvziozrr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gycdgqfyt.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gxfgodzjz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gimywchsb.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/ghdbbhgnt.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ggetifpre.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gebvsffcx.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gxwzmpcdu.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gakzaebso.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gebifehyn.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gmkditcyv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gebijfvja.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gorbyrmjx.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gguubwfqp.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gtgzaogjw.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gjtxpxwcx.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gpdrzvbwy.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gizfiwgwx.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/ggrtjsxya.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gvrubyvmm.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gxdztkofm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gsbjtgbak.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gjkvrioma.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/glktppmif.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gljdpmtip.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/guvehiprv.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gqzchsnpy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gqwrkxopn.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gsxfaqydb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/ghsauknmn.sHtML


<!-- 参考信息 -->