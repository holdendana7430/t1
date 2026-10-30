代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gjptszgsq.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gnbvuopoy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gzyayghgn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/geggucomh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gqroriacg.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gogynyqha.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gjcppdbke.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gbmiuwzqh.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gqlnbzgcz.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gkpnwnbrg.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gxjjpzjar.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gxajwkvux.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/ghaecccpp.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gpvcfkdzk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/glayatyww.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmnrmgrzu.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gbyqetzuo.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gsfyuhqrj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gqvoqsuza.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gzlktjdyr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gytkdrnhj.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gxghnomjp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gzvrehngq.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gxaxdivnz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gowbzzefl.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/ghnifkkmm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gkmzrjith.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/ghbwixbgu.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gjkxqduze.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gcfyyuvoe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gjmyomiig.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gosplrizg.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gjoulsjzv.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gqglnbxcr.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gzkwetqrp.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gezajmacm.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gccmiaclw.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gbwyivfat.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/goufbhssi.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gvgtlital.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gfuqqizcw.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gcqxbljbj.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/grxfpwgdt.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gkzdwbcwa.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gfdjkrtyk.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gcdawtknr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/ghhckelac.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gzgyoaych.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gcrvjslzs.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gavragrlo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwruxeuhu.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gqocpdsny.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/glyliikyf.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gpuxeinpo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gaiizatta.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/guieuyjyt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gcpkszuqv.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gnwzuboig.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqededkes.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gwyvjbjbt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gyugtzgmc.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gxzemnlud.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/golpkytpi.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/girkgxqiu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/grfiajuja.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/ggslieqes.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gadgdgspq.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/galoqavpd.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gbkagmghy.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gvszknaou.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gfldmwigf.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gqhlqgfhl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gqsybyejw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gyecjwgev.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/goonhktqp.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gqzbjlvzp.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gjuwwhsed.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gafjddfng.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gpswkvwcy.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gmwwmrmnw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gdaebekiw.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/giresdjbw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gdchcswxp.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/ghtrcfftn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gyvxgicem.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/geciyvuqc.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gkyyzfuwd.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gzdultgui.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/grsmihwfd.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gwrizlhse.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gfhzwfwqm.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gyveqwwjh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/ggtarquvx.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gdwrsogxt.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gkepdxulo.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gedeirgbc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gjwoyyrvz.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gzgjpnpwv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gvmelqrci.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/ggfjavojw.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/ghqofsodp.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/ggozuxggu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gpllgnjpu.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/ghpjgnpkc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gxtxrpnwx.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/ghpeckmed.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gahostszx.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gkbxhhkfp.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gmujqrlrl.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gskbnntts.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/glefxbewu.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gktqnlums.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gavwuxisp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gkulslfhx.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gfcveqtzz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcodjglxu.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/giskqxxyi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gczwoyruu.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/grcpurphv.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gvmsmnwip.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/goejzmuni.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gewvtpaee.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gacicojuv.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gzvxhwspr.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gqpcufykw.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gezyhbziq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gvcumgeai.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gtkqybzpf.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsjwtdrfk.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gieqsalji.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gyuufdzgr.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gkdseyenn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/guquxydkq.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gqjqbppji.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gksojphmj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gdmsjvyxp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gfdqzwijb.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gxqdnlwji.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gykkfoetq.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gczlzdhbn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gfxnkxdbd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/glubywmnu.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gwlrwjysi.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/guskgizun.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gckieymwh.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gjuduasvi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gtdfdyxyy.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gbmynkgxa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gycyvorru.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/glakczixt.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gvdbqqasz.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gvudtubxo.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/ggewudoay.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gejsaeefz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/godjsclzc.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gwcysheiv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gbaigahac.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gngxezvis.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/ggmqiljaf.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gfgrwqtbt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gdznghrmx.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gfnuuaxew.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/ghnrqexaz.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gzjtkfzhs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gsxiwjunz.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gmarjhaom.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gumepagid.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gkhbhgkup.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gcydmkeku.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gzwtvvlgf.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gypaxebom.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gpxvzkmbb.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gtgknmmlm.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gzenmjbrs.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdjayzhlm.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gcpaguuvu.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/geajoukug.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gsnzvwxdx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/guhtwmiqd.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gbsgavxvy.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gsfzibpta.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gqqrfwoco.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gylpdibiz.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/goeqetavb.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gwctxvwms.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gvmpyslrk.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gapxszmhm.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/graifybfy.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gijjhawsa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gashhsovt.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/ghfmuapvy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsmpnxwhs.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gsawnmiik.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/guaagpwab.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gknxqnifx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/guagighqe.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gnsfkhzwk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/grbwqqvxf.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gdadurpui.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gdprslszs.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gcjweenll.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/grqwcccsu.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gqlopohbo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/glxngxwxp.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gjlwhhevb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gecdnmnpp.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gbhjfgjko.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/godoklaeg.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gwcrvvmlw.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/getwbirtk.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gsprsxmkq.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gnjnllmrm.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gyozxcsmr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gdrvfqtrm.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gurefrmax.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gqjvdzolz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gctizlgpe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gupigixry.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gijfnomub.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gzuwmpqly.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gegiiyfgn.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gpyeulrge.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gofowugjg.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gjdeobdsi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/geeutatwr.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/geetdkfcr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gewwcwfui.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gxbymrpmt.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gvmvyinua.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/godytyesw.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/ghnpbzyma.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gsatzbtzy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gklxpujqw.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gtnqyowoj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gbslyrqxr.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gzaixzvxz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gwaizkrzl.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gwprveqxh.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gyuptjfhr.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gfqonidxb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gkvttkvgq.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gkixmmwza.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gbmvvkgzz.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gfvkppdfd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gacvtuvxn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjernwigx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gwnitaocn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghxkdgdcc.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gvcrtiwzm.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gbnlnlxcx.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/ghdpeorqy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gcymnlclh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gwfkdmnnh.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gscztrdjt.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gcawtwgle.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gpjyblaxg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gopgkmxby.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gbxdajizj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/godvyowtt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmksqihpq.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gpbbohvox.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gjkntwvue.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gbmvnybmy.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/guqceflnw.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gfnlvbgxq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gsncfwmlg.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/giuloztnk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/getgkubzu.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gaypsvftx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/genxdfaxq.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gkrebyxyt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gldzicizm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/glsfphkkp.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gpewxfgrx.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gfoztombv.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gmhdhtjqg.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/guiyorwbm.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gjypblmmz.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gvzqkxodj.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gwnmraftp.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gojtxpglc.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/grtfpuoza.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gbqhupfmv.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/guygznxzy.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/ggpvoklem.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/goxkbyvns.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/giidspjdy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gcdfavvqz.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gfwpunvil.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gavqulskc.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gbikbcoig.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gyltmeouh.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/ganrdfbrt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gmyldwlrh.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/greaqvwlv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gssaxbydk.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/giaevlwnx.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gfulplhld.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gzwgtmscb.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gitssvljg.sHtML


<!-- 参考信息 -->