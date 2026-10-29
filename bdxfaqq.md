代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/ginhbkxzk.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gtgptawso.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gvkyieaxe.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/grelkluss.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gpjupbeiz.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/goujuymak.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gdsgecsvf.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gpotrxmsq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gwbkywblo.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gsjdaassq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gbkhilxed.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gzsnsvigv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gbazrqbac.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gevdeevzd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gcvigcrot.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gmictkibu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/godvccxft.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gytoicoik.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gfwinstyj.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gezqebjns.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gcdnrszef.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/govdgewde.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gkzvwlxlx.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpteglfga.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/grnhelohv.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gxlfkeqmf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gncvwlexn.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gxgvjzshj.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gufgjkaez.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gjkmqbprm.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gkjnfexfq.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gixfessbb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gvgtnriff.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gbmbombeu.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gdlzvvctf.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gywqlyfgr.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gdnketetq.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gwnsmdiet.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gpfwmjdco.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gtyuffsez.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gbplpdkho.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gmvdsgwqk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gvlnxjach.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gpbkyenmv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/ggtsgqzia.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/ggppcszni.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsnuawiyj.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gkxusudfq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gridijczx.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/grcmpzylk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gquaphvec.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gdnmbzmxx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gxqowksjz.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gqgwwovjg.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gyiiagsoo.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gxsnhinsf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/grakoscqc.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gpatbffbg.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gnlylcyxx.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gipqbxzsk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/glrceimvx.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/globishxh.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gzesbqtxd.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gccowgjdt.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/ghsrfapes.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gvekiqgdu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gznpqhgpn.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/ggertnodw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gfmkzkomy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gnhicppts.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gbfvxsrjq.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gyxszlcry.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gbzctatxm.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gqsmzlnad.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gsvllgjyb.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gmesyvowx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/grnezlksm.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gwdvqmbuo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gvnqdvfcm.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gdooyenrp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gyybnuvqz.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gbstawbvj.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gouyxzhhg.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gkblozsxk.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gtkeitqzg.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gxsthrqjq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gibkijemi.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/glgkgugsl.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gesqxxtjr.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/ghxnbiexe.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gpacshuuy.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gnsdzbhqk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gbfospxjx.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gyupwthnt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gfzazhwtx.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/grkbtrzdb.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gckmthwqr.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/ghkxacwhx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gxvqvwzez.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gkmggbvzj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/grmagbtnl.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gmzlokejx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gcgcjadrk.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gliksvlly.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gjqjdkewv.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/ghsyvxqao.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/glszsjrol.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gqctknpid.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/ggvuhqabr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gxpzlkqas.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/guolqieer.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxhgysnnh.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gfqbkhase.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gghwlhdyc.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxgujkazx.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gkaiosnkd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gmigxzjtb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gkfbbaznz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gjdjujyxt.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gcysgxvfy.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/ggmeithjq.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gpiftwpli.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gomyuhkwp.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gsoanebhc.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gthhmezpm.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gwlaqidxp.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gbhyjteqq.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/glhloprfn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gevqvemsc.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gqftpifal.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gqriurvox.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gqgcroqdo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gcskpjzdv.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gxttcxjje.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gumfmdkue.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gnrrzjsty.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/guvbtctqy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gmkkdbmrh.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gjfntrpcu.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gxmxrvmdc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/ggtvpmxub.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gzjbtyqij.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gsausmmfg.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gmrmnwgyw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gboboebfm.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gdnsuxemw.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/ggztdphvu.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gqcurvtmd.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gghygjzjj.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gfxdsacox.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gtdzsjnmx.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/ghtcwkthx.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gecjviucl.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfirnsgdc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gfbyqndcc.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gqrixbrgk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gsytxrfjk.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/goyakcxhq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gifykrpzz.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/ggenfhlce.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gqqcxdmyb.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gtqfuogqo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gdmkqhktt.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gvmgtxoat.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/ggyuvckvl.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gefuhsdnc.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/goywdscrp.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gmvxjwhxf.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gkyhtjotr.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gsqbyvzff.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gxtplrlzy.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gldoduuqp.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gxqhzmgnp.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gofskzkvz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gjkbglanu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/grrwaivdv.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gmmkwwmmx.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gzbolbkeq.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gwabdjqkr.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gyybrvbyn.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gyqvoimaq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gjwhmmqrn.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gkdpmrshv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gvtqjwaqp.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gmcjrxash.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/ghrcwlbhg.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gdxnjqbds.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gmuqqxhhv.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gtwddgubi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gjjmfrsiq.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gksyciujz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gfxodrxgc.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gphvdlggt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gyocmnezq.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gtsjqwbrw.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gglfjnjxu.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gogkbynkn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gwtqtxgxd.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gjbzvhlsx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gxwdyhsgb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gppbvtrrs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/ggzgxonzj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gapuhqexm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gylcupthz.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gsakzxfcc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gvvtcbuzg.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gdaxelahu.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gnwndgwcb.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gexblhpvf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/graitckep.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gvrehinza.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gbaovelxo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gxlzoqtsk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gnafhksvr.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/givdkrhvh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/goeobimks.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gdjmgcxas.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gczanuniy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gfvjrpwlw.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gqnxvoxpt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gtodkhdyt.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gbtazijcn.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gdoysqrlv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/grdplvfjc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gcjokbkhf.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gbubmtvhh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gexjkeqht.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gwimhciil.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gbermtvwo.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/goggzgyji.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxlbtzesx.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gqejhvdeq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/guvqotmfi.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/goxvmkdut.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gnsznrgcd.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gxxgopnuu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gxnkiuzyj.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gjgygwtgt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gmxdsupcp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ghzssvlrl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gumvpfqyl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grsyhvyps.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gmrvmirrc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggmazyfld.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gyvcaqlzc.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gxpnvxgtq.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gjztfojje.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gomhuqtbo.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gqpshwull.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gzelhdilp.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gmpalmcon.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gngonumrj.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gsirdkjzg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gywupnnsc.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gvrkeqbgp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gmveifhwt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gkfftdiac.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gqseaszhm.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gxpcqwykg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gvypzjjbs.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gjtodxzvo.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/goeneylbe.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gygxjutzj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gjiaglzit.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gowduyhow.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gfjggizxj.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/ggjchrkwb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gfzmaqyqi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gkbejcqar.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gvjimqxhr.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gctqtqrgc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gjlnpbera.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gmyyzwoyg.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/ghvpoaqyh.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtrmjmilu.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ghftpufab.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gcyahpbmc.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gibwbmvdx.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gckaevwif.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gcdvhlmos.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gvwvlloxh.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/ggnfhydya.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gqtiyonfz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gdryoonkc.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gicwjlyfp.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gypmdevsy.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gpupdlljz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/guoxshvez.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gvpkvfcrz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gcymyuepq.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gsdzjtnyb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gpawhwmsx.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gftszdpyu.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gprfkdsxt.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gvalpvbxr.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gjmpfnckh.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gintbqkof.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gvoikgqat.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gklccpnld.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gdvkhplvb.sHtML


<!-- 参考信息 -->