代发 wailian999

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gfaarykyp.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/ganhmpudp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gqxcjlmvi.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxjxbqgxm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqevmgts.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpxxszmq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gauulguhf.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsezvwmjk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdgkmhprj.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gvebchqwt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsovgsuxn.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gauvbknqp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqhoxaxz.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsogxjgc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlnspndr.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/galaygrpi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gswqjomnb.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gnciuqxlu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/ghejpgyxa.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdkmyxmkl.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdmmgpgim.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfuwtfwa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gzjilcdfr.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gllczhokv.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ggblaabvk.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gikytijlc.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkrrskfh.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpzsxvso.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gxjkclfuf.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gmekzcjok.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gaorgbkga.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdblskcpv.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoorwkki.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gicdbnnvm.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwseudru.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/ggslrhmka.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gesmdnwhm.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaasxytaw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gzaxdbgyx.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbvshqcpq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzcaicwpi.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxryljoyc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsilchrd.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpjptlhrd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmgtpskc.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gxpxcbllo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvflatqfj.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/guxcigayf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gmbcwljyx.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwdnlfxw.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfybdwbr.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gdmgqndiq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/ggpyrfeip.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gudofxhdj.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkceviciy.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gwunhzsme.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatyqvrfs.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gwkhokmqb.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/giopyokcw.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjyqqcrf.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeslolhj.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoocrhhp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gcbjbebwn.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyptucvhd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/guwiquyvn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdpqbvez.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gajupgvdd.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/goqocphje.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gecpjtgpo.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwxmjvyy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxmfoere.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnafffrc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/goeukjkai.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gyankgibh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gjmplgnde.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclrxoucd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntbzdeny.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gfekgsrwu.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/guanxiuqz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gglebarjo.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gfqcrmaba.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gwtdbdmdw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhzdbkke.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/geetnzyoe.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gngquqyrw.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvugrpjl.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmjmuugo.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmqudewaq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzbbgxgv.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gjuacsmxk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gofpawomu.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjrvzyww.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfoysxqw.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcxwxyoc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdscsque.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gycebgkmd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/ghgahbizw.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/guvygtryq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/guqjtdzen.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gdyycqvfu.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gqipzaifq.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gxflusibw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjcmbamv.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuxnvlvg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqfctbjoi.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gjmpwmauh.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gzpidlmmu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaudfirhf.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/grtltfymw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtendpayw.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwnczunl.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gpqrvyara.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/grtbwtbac.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gsnycfcls.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gfrwexbbi.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvapgoub.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gguzeedzo.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gllqquoau.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyxplmvl.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdvqjvpda.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gwwjvyjdj.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuhsxmet.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxnandai.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptxtqgxl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrtvgikg.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/ghmrwminu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmowonub.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/guqnsoavp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmdvjtfl.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/ggmxvdsyu.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjsticsb.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzbhpmaa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gofcqdxqj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/grbhtojum.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhvzfnbw.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrvnkrce.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyxtogos.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiwxdanl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiyjsmnz.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/glzjsvjdx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbwtinwz.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcagnfarf.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwzntxjo.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gkauetrpq.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giswuxgng.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrsfbnuy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtsprdrb.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjzhdonnn.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfmrmrdc.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbzgbwjv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfcaxopn.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gwtiftyqq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjqlwtwe.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gtlezvmij.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gpjobyxeb.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccquromm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gkuhtbngr.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gonojrfrr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gyvjqhqua.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gephhvcxf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkooafab.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdwkysjo.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkpzzyet.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerbxjxac.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guewkwjng.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gjuaectkb.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gosiczgea.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsfzzbhvb.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/grvearyao.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbtwwkpu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/guwuzyeaj.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkajjqqz.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcznwoem.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnvuqrne.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glttjtpug.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/geoyeefiw.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeovvocz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwmayohyd.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glvsrxovk.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gxgeeyalb.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gtshcvryw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/glkalnfxs.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvnqvznm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtougqwl.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gcrxszzca.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gebjijres.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/grklmdbms.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/glctensaq.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gmykawlsz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcelempq.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gylchubfl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcfenikf.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gcpnqvltd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrkgdbzb.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gzkclzuol.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcjdcwki.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gixbzvijl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gayijxtsm.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhosongi.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gnfmompea.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlsurcrx.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gizxpatcb.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gozvuchzt.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrdyioge.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gumklsjnh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbchbzruh.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfwniuza.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gudrqvipa.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gbmvfouxh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvnuqvbj.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfdrwtaw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gnbgfawct.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gfkevoeym.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrcubowb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gyvqqnexg.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/giromjrlt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxxucdpi.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvndxzxxe.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gspydkzws.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/girzgwzhr.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gngoffmxw.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuwpielk.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/givsbqznk.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcrhblhm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjghjxoe.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gewtrhjeq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gqixvyfjn.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gayqwqmmd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gychbaaks.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchfixpum.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmbwmkpg.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaxahrqj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gmmlrjdrm.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gdisbascr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzxhockw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gogijqmiu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gabizupzd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcnjlowc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiwpkfve.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggdklnhnx.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwqeiwvg.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdnjemuw.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/grqmcjnyx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gdxaxintx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvqurnwe.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/guehertzm.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaguelna.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gfjyqjrkz.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiadfdrf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxwenuiy.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gubbxkggz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzllfvdwz.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzbbkzoq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gboaimnsu.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gptefbweb.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gljfhnzft.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gazkkjlvn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnfankvl.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gceqtsfao.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/glqlhkkhv.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gwatixmpj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmtcuvjh.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gehnatujp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhdfnnxd.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gklpjfekb.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjjidybh.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gwmfxldsa.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscootkau.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzechmkme.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gmdxrfpur.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gcjyzszny.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gjpprbpqo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoewnkjr.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/giucrfsnj.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwdalgxq.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gwvwuulhe.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gkniwyfvb.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gjgqlpyrs.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gctvvfayc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxevplxx.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeblwljm.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/glcalultt.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnmotzkl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxnmzbgge.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gotfysnos.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gewueekdd.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqyqilqu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gjxsbssgi.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gsxtslhft.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/guupjghlx.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gqslbkoyo.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gjypxhdzd.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkjbmljd.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gldzibnfd.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gjfpyitup.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/grrjyroeh.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gugxbzhom.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwntgilg.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcjjupqt.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gbztnhouj.sHtML


<!-- 参考信息 -->