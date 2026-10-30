代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrcoikez.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqgfxyymg.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gshxsbbio.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gbxibjdzm.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbixvcpu.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyrqvohq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqfwxbej.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnynjbrl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gnplcczqf.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwidvccg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gdpzhundx.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gywkyqvqe.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsizehkfz.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbjjfxuz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpgwphiq.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gyumzmaii.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/ggowtwlsq.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvpwddxx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwmnsflwk.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/ghzkyeycb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvdsjwak.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gcmirtbsj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gmapgmtlr.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynckfxof.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyvujulp.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gwytabvhf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gwmlnwtqm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffxgqidl.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtgaclni.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gccthnkze.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpdnxvpu.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gwwscnzel.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gujdzqbci.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzezzywme.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeryubsz.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcxtsqec.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gnkcypgsd.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gycfzekwc.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/grobqbqta.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/glcrtsfhw.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgvlnwtf.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gwgdekggg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gjqtnxtcz.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbraycudf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxbrejjn.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnbpucwb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxbgsnjk.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmidroto.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gblnkahtb.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gtywpdbvj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbvfebhw.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gmohvuuie.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdldujom.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/grnmobzsk.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gftmhsmkw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipptfsov.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkhoahjj.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghiluzjjd.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuwmfyiq.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbdmeaox.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjzjhuyq.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gytcygfkw.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gvessgmcs.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrarqrjc.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gflhumusl.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gywovojty.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbkmpqul.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/ggavlwuff.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfxpneya.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gafsuxfvw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gldebtcpb.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gcuoglcam.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gjlznfjcv.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gowjggiwr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gokzihsws.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsmgxgml.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gwqqfmkqt.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gptyrrwqw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsydsmoxn.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gfrbgqqjg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyhneccx.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gqycboupv.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gvryqqcio.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gzjddlrzc.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzvruxvo.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvjcmuys.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsrbqsbf.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkirdmhlu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxtsqqqr.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwqbleio.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzqqnudl.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjqjstbp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyxptpvx.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gfupngzqg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/grvkgdbun.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtujwemou.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gwezvmqbt.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyahovzg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/geujtvgme.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuqipfvc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyvzppdj.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrproqqc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpkgiepb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryavhhgj.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvxkrwxw.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gibajrwiq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmliojuha.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gxazyrrwo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqwtqpra.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/ghazaowdo.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gjejuuerr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqqsomnl.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/glxoopdtx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grgudpyvf.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghktonypq.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmbcziqd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxjriiocu.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsdrbqnn.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gavfncsmm.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/ghqpattry.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gqqhhcknf.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyylozwuh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gppisakom.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gfxzkheow.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ggxyukuhm.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gamwusomg.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gmsfkgprw.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdpdvbbs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/ghymzsnff.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gixkdlvqz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gulzyrvqg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoafyitp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopillgtx.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gojutwlbl.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdjplwzt.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqurhkmm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxyjnewg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/getwiclql.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxmrxgvw.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwubtyxr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwobklvvm.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gydprjsoh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gygdpnmxb.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gbndggwbo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/grulixssh.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gdufkxmjs.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwxismxm.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbncjygu.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gkevznlpv.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyjnhbhh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrgzidlb.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gafsilvgw.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/geucczkpm.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpuhvfjqp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmkquoln.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwvntwmf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gibansubw.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvqkdnmy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/glkiytmcs.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gjopeucjs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/ghwxrofdp.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geekivdbh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gjgzodzbo.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gjrqpyuuj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/glvulvvpw.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdwtruyp.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gukvsggbr.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/ggzcdkkjz.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrklmvhf.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevojbykv.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gswqmpxnf.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpvuxtog.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gesscsrxi.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfmmkazd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkdwqqcv.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gjvnmovrq.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gyyvlwfhx.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gpliofyog.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gmyzxvthl.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gwujkeeym.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujwhedeo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gluhawjgp.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfchqnkz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gswdfxjya.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwbwoqaw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gpolhdimy.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrmmxxde.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtfzhqpy.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gucbojxku.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexssihjd.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaqciode.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgrlrclu.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gwrzwmwpo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfycjzjn.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gcivysahl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glchekxsf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ghacxdntk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmjaykxw.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gubgujzxx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/guwlmymws.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/glofjiofk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gdiqbovrn.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpcbcrcgw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqfboyfg.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmcseuzb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpldblbr.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gvthnowam.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpdcquol.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gtyoygcym.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gbcroptol.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gqwretxxd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsgktplly.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gosiiupat.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwfuijflx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glhnzvonr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geutzdldk.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdflccjha.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvnqpcow.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjcrttqo.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqezrocns.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjbttljz.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/goywkthhl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnivrhcxk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gllhpksgb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsmdssqnp.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gltqlfopr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhhlkmcb.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobaxfjfb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkpbfqpi.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwhoiyjs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gfbzmlkuy.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gztcqfktr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghhwtloid.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gixzzbmkj.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmclhailb.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcvplnvx.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gzuufnyaf.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnitqahj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gagmetyqh.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/ghbowczxx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaietociu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbdvslnp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gsxkfjydd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvymyuet.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/goagpzleg.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gyahxjfxw.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkefufnbv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/goioaohts.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gogfwkzbr.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gquontzrp.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/grfdzjbti.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gutnzubyu.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/giphxzdeq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/goeixyovq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gqkcfyzqr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gayjclyfz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gntyykfiz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjljbdxkb.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyxpljqv.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gxxbfovtp.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gidveeiug.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/ggexcnrpb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkdxrxjlp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/ggqelnirk.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjptwbck.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glehyghlt.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwflzexrf.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxepwweg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfwotvvc.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvbwrahst.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbdcefjs.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gsxqdtkzr.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeshrbfs.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gnyycgamf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokjvpxpu.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyqpkwlj.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gslemcrae.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmhggpkd.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gezbnhyqe.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyphqzmi.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gywsjdvhz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqqkxkcp.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnifrwmot.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrmgckrq.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gsvuoygap.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gkjwonnlc.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsxopvqw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqcwaxbt.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghelhdbzl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/guyhcaghu.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxrzmqgk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gffxzfksj.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gokmknthj.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxanablzq.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gotqvwdvz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkyuyagb.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhjqpmvi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzstrwlro.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnurkgdq.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gjhzasfrb.sHtML


<!-- 参考信息 -->