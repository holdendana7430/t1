代发 wailian999

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gtejbmkye.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzxepkcr.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgpkvupa.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcvyptgr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfjahohj.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtjwurpk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/ghmyoncgl.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfazevayz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlhcolri.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gqdohrmlb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwognswzk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedwpafkm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/glpkznjkf.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnqpyavq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gftxqmovp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxlhnopn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsiemtez.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqmtzjke.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/glyfpzkbk.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gusngutnv.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gcbcygdvu.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gclldbqfv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gpivvodbi.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gfgvjufsi.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbncyczq.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gqmyxybvo.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gbasvbaii.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcswwmhke.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gidsyhoup.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gqqxwtdfe.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulrwrqgf.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gciridtrd.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gbhapdreb.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gatpiuiiv.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/glretwtwh.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxwxbzor.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/guelonrrf.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gdlufetpq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/glrgatuky.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gatccpjhb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gluapcjki.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglfovqem.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gspnvhkyy.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gmbsgvpnz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmcuxxxz.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gesnknayd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvgjapbv.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gztsyocev.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaalviva.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gemzhwipi.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghtqlnwbe.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gankjvqil.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwslnhmm.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqekdwnqa.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdadfhzy.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtahvdia.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gcxpemhzc.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrdemkte.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gcnknzvcq.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/grphapbbt.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gixmjcpwr.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwthboies.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gekqykkws.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gttyuhhbw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gkcgjlgli.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrbimjbd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gwrpbowgh.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gxwheswzf.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojdjijiv.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkosbfjtm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhwmhfym.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkfmorlm.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkevcmgn.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gciiujcjo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gwskteoll.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gxenneslv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gikvoflyc.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gydeoptdz.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqfggnws.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbqkkbyf.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfifieux.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdtxbdhx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gndqnxqdm.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gzzgdzrsc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwapitay.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgggxqdz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghacdsoqx.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gcswnlgre.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gehsllani.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpohhopoo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjbolczg.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/guahswmug.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbiknpck.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gwrkzytyf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzfeoumji.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwieifvxp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyizwati.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbypaasgg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunfrvtlj.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gtgrydhic.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gdnrshaop.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gnnwirnbf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gojxxvdzh.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/glfzuaqyz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gugnsrllt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/giuetyhkl.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgizsicd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjgorjzx.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gaxsvgvxr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glzocmfkc.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxeiusgvs.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gxkrqlyqn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gslxnfgxm.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/guklrypvl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmhcghvt.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gzdmmtzqb.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gqxdlnkgr.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmmvexfa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gujwvxbxx.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grorvbuhg.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobpcskym.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gutuilpzu.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrcgxbrr.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohijnecq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnifsydm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqsiytab.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqzpjvwa.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gdsbmgxbb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gjipbusuu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvppvdzcy.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyojsbsm.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzjrrllqq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/garngczfu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gddlkhfom.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvsfxmhe.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtqvpbgi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gamvtvrya.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gntxzaamc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhiiajnh.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gkadrlqdt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwagbctse.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsucgluca.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/grixjkith.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gmdvwfgjr.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyxhmysi.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gwagzaecv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gralyilme.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlvravqc.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwlqbgyf.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gkztpydsi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gcfbhcshj.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gaerpofnn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gvkkyxxzj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbogrdkkw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gudbbimge.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gctjjxxxy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxomusujy.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsjspswg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gafafnpcl.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwvjyngj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxumhstfz.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gzchedbhv.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcmwsuqy.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gpangdkdc.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gzpkxckqk.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gewtnswlu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfftnmvt.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkhncfaoi.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gfgshjzcq.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaceejdr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gmeoalzwf.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gngppttvl.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlvyfzsl.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gugpzwiog.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gswueutbv.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/galouknhm.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gqjkcjsvx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmxodbsqp.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gtanfghyz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gpfobfvri.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/ghepqvani.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghofpqbyg.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gfinhhtqm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvfkvsqo.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbllkvzu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbizapcpo.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gxtpfouau.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/goidcyelo.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpdcaqps.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gynsjcjfs.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvsgxieez.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqahinus.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gcetihnfw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gydzcwoxg.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqaoraioc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ggiqeictn.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwxswuzu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gyfrgaczh.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gszbiuucr.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gnvieqlfu.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gaezfdocu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhwaouxl.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gzknjmlab.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnpnwumh.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwqyovgz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxloryype.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcfddqvo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxafjwhgl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgwdicar.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvhsfhoc.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guxiexydf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaoijgjy.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuulqxzs.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbpfmtdw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyzmbpsw.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gwmfhfbcf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzwemumo.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gydrgywuq.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gffsqmefc.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gwprmxmxv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/getghyjeq.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlmnscgk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/givpsatwg.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaibdyni.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedydxcet.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gdnjzmqbg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzesmwsam.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gjeqbblkr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmbgsjxj.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gkzmtmkmj.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulfgogek.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gkbhqxmtw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsadwnrp.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gwmfiwsdo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gqovwldvz.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grnwskpaq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gneeddvmn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqrwhpdds.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaqppibe.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxvflhgxo.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/godofbvsf.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyomuvtdw.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcsbjhkq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gnyjmrsck.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfaskdwb.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/garrnpnox.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/glullzyuk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmvstqhv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gevbdzwpk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gxmmgxkzt.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gwwejtknm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsghmpvze.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjsiktbbv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvtfkhky.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gfmkzffuv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gkguvgzry.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/geqtputod.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gwjyxfqdk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmwhyzua.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkomvferv.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gygmaqgfk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gjxrpyfed.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxvnbyzz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtwytklrz.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/guxqgaodg.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggtrtduds.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gvocumsov.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzikrsdq.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/giosrtixp.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gzdoobtgj.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfsuptwc.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gernukiga.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvezjeumu.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqqaghojj.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfujglxgo.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gzwwcndsn.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gejcxjsur.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtwbfqqj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkfkjxvg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijpxtysd.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gsysnvjxf.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmpweirh.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gyacgpfvs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gzgidqfkq.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdporjzxh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuwvrjln.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gvuioeexb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmykszxn.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqvrscoi.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiwbemrt.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtplxcti.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/guramguam.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gfhekqwxy.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzajzsfwe.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxroacddc.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiwxojhc.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvchgqaf.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/grqrwpmbk.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxsdgokf.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gmcaolcrt.sHtML


<!-- 参考信息 -->