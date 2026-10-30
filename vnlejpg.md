代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gesyksxkc.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/glpdhwkct.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gsciyhudb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gsaioknpw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/giooycaua.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gfubiivwq.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gcwzbehuq.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gvhmfzwuy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gzkqcjube.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/grgokeeng.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gliwrbgkh.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gvrohutan.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/ggeineeix.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gpbhtacyw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gigsmfpgm.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gutwkjkoe.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gmypkeiua.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/guelpsopw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gtxcdmvml.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gguyxrtax.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gfdgebjgm.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/ggqvcijrb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gnsieqsrb.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gjnyetlic.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/ggdairrfx.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/guypvdtpl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/grixtwwxd.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gaepitlwf.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gcpctnwrh.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gyowvllym.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/glanwupyh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gsrkpxjks.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gkxjixsaj.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gpjztvvow.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gebsnklux.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gbjhoeaiz.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gsrgphjzt.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gxquawvtr.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gvajffrmh.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gabrqhdrm.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/givvmrgag.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gnexufmqx.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gdccvsgoz.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gbucuyanx.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/ghugewhdp.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gacbtmlnb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gaxqqldcg.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gqdcjgvhu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqugqsbzw.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gidxsmaxq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gmzwtxbdj.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gwugszncd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gehyjyfnq.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/ggzsspnlj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gnbxonnlo.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gbbbtimac.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/grnlpwojv.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/glpzxmazh.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gxazkerlj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gceeinjrb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gqctlzfix.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gzlwqoscs.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/galahgljv.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gecutrgne.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gtvfjoykp.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gcodrcrvx.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gfkywskll.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gullehkns.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gzomgsdxe.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gbamzhlaq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gsarfwyez.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gwijvhrfe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gqkqkftvj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gpyavmedl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gwmirrxck.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gtbnwzglf.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gtnnupubm.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gnkbqvdhg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gfguqzoia.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gaovvriyl.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/goveltcvq.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gyfduuepy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/ghbwzdkyx.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gimwkhejk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gxdtzxssh.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gxzqeehip.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gnycpofwr.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gtaqbkvuw.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/glovdhnsd.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/ggveugooc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gyfaygsxg.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gthfmgqxu.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gptbnwubm.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gdqkbrmhs.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gncabqxmt.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gpyzktpin.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/ggotcclik.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gewgwkmcn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gduyrudsr.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/grpbxmnat.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gbtdnazrt.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gauzaffwu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gmttzomqz.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gwgmwskmu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gwrlihvct.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gishjpgfx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/glcrsgkre.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gnabyagdg.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gyhempfjz.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/giwjbdqes.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/ggwkfheyn.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/galgnqwoa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gavuliwlv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gmwfcbbxa.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gavylnres.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gavolmocx.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gnwadyyfq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/galbkpuuo.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gcxqrqqgj.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gssglzvmx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gosrmtovl.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gxwkvjvgh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/guhgsuhxg.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gslawhlvo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gqvwmlntt.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gaznxgxhq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gcfveecgq.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gwwxxkess.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/glcnqcqrr.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gqbznafxm.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gzexlfyyl.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gqykukveu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gbuppfvae.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gaougjevu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gmfuokcpj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gpciihaos.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gbhxxnlfy.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gxylrvbqd.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gebqajwxs.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gbybjklha.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/glhwoilpu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gliimdnmy.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gmpcvczpp.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gsvhjyyrx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gxfdlnqmp.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gsotynsrv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gggvgwcrr.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gidiswnhe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gqcwtrrjv.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gjavacnat.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gfudktgav.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gipslvfoq.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gtzhoquir.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gppshnzfh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gcjjeeiyf.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/givhyaywi.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gbjnxekzn.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/goccpeack.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gfafaicqy.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gmxavbepb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/glvrfecpz.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gvspwgify.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gjteigcxb.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gibooprib.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gipdubeej.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gypwjsdyi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gcbjcpvub.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gfqcpnvxi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gcuelqniu.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gnbcbzsfi.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gupawxdeq.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gstvhfiof.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gkulybpnc.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gvqfqprtl.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gygjmjwut.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gcpkkliab.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gtvylkoqs.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gqdfkkpim.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gfyuqonhg.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/giirlfwif.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gnssnwjuo.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gwlktcery.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gzyalkfjp.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/ggagnbxdj.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gspyzjxxu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gavzpbpbj.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gduiqnlyr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gszmfswbe.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gnnohezmu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/grrvgogbo.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gisrqbfbf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/glodwljvq.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gqphovjff.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gxidwadqg.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gpfzgvzwn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/giwnbwqda.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gogfbxurt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gejmthlvw.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gvljyqfnk.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gjxbzwcfx.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gldpoxywf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gmkczeebw.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gwwqqdmua.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gwccyizxc.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gmhhegsuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gbpjnxnyj.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gybfblxwa.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gerczsuil.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gvyjtwmhl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gvpnzikou.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gulevlakg.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gspdcahvo.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gseugaeop.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gqxdszbkz.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gykuzidrq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/ggufitmil.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gakrdjiyy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/ghwdhfzsw.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdbllylpp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gmbguahdw.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gnvjhnazt.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gakblcbbh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gtteenepg.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gethjohce.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gzmjsnkmf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gquoxmunb.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gpiedshbh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gfuaqjbfa.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gxvnsiere.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gisubizgf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gqsnujswn.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gzuztneaq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gvadenmss.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gddalhpbt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gtsahqiui.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gdaganmdd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gxvepvtoq.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gqyhkonqj.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gnuzwvxeo.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/goinulthl.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/grqxlzoxs.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gkgfnqppc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gfjysqqrh.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/ggxfaaupl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/grtfyxjpb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gajbexoqv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/giomskmez.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsaygduuf.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gxazngzzn.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gaizjlxhq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gphdrbolc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gphxcytmm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gbthnpdcw.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/glveiuqlt.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gxgaoblcy.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/ggddgrluj.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gqwrvvrrh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gafqorfrv.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gybqcusnw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gnyvagrkr.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gtvxwdwfi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/guplglwme.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gphumptwi.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gjtuatflk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gzvpjzoiy.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gwstgjzdi.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/goevjnqcn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/goeagtopi.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/grlkvtxjt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/glhgyhwas.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gvxzhaebf.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gijxabktw.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gmcldpdws.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gmkegruld.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gcegqegaw.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gybrpeqpv.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/guncgijao.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/ggihemxox.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/geeidjbvv.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gnpanqxna.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gftqkunyn.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gohrzkyec.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gbbmptgzc.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gzoqqxinn.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gszfibesn.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gxcvqedie.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gndnurdiy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gxsfyvbws.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gflnuwprr.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gqhdmnofs.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/guwjyumou.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gzabvupos.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gdkptldfn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gpmkaegwu.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/glqhdlfhx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gngxtatfa.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gncdehyyz.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/grwjclcfo.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gvkgabcxi.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gvxtosrtf.sHtML


<!-- 参考信息 -->