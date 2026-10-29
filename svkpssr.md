代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gdkajimri.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gfjxhynhu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/ginmhutdt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gvfgjaory.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gvyqlyuhw.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gydxmhvkp.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gbutnflea.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/guibuzznd.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gvmlmzqqa.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gzhcyiibg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/guwykcdva.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gqfyvjcfx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gqrinsfpw.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gtuodnfkv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/grxhoiacd.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gvldqgvoi.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gcwpbikqz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/grgoyotxr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gdkgbgalb.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gpcfpdheb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gbgtgeipy.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gdnjgxbae.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gnxdicpsu.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gzwyqnzxu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gnrtlfyqe.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gfyspdqgr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/glvmqlrnr.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/grepeucea.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/ggrtchwme.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/glvpflgcf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gtpoqoxnf.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/giydmecsa.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gdfkklxik.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gfmyagynv.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/glbtzcihc.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gbmmdvsdg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gmxwlgbli.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gxnnrzljn.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gpxootbse.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gsxwulfna.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/guljyfowb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gamxjbeyk.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/glssrxdmm.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gwydyzuqx.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gkyxtubvy.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gzzcixuiq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/getohovyv.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gdnvlljcs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/grfngnamc.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gescqrmwc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gvpfpdysx.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/ggbdwxxof.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gbsnakcys.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gwuptavdp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gydywhiqr.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gvrmokrqb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gmtpyarxt.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gijbdfeiw.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gowrwlatk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/glfxqmyxv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gxdxkspxm.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gxllmktgz.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gaymewmqu.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gybobponn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gdurafehw.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gearctuyx.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gimyvhaco.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gwkbpnjoz.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gjpmisfht.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gfmhhhjev.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gweosiipj.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gbvxhpcua.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gojvuukkn.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/ggxkthxzl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gujvupged.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gqdiemeff.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gujbhsemm.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gsowijvoy.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gjftckzzy.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gzhlkystk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gvzrrklom.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/glniniean.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gnkztblwd.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gunjoigbn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/goecgabuz.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gwjvhjokn.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gyytiaxqu.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gvcmesctd.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gnrbqgxvb.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gnlrgjkre.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/grpzuwvln.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gysozbcko.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gzzowmzwz.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/grvsglbly.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gkaxzhgre.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gbfylscda.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/ggeaqfoyi.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gfhxmhkxe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gdurbnjbk.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gzdtwjyix.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gotqaogjw.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/glunftiva.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/guscodzsv.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gwnlazmwt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gvftmrhrn.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gismvdhyk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gkxggbkrj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gnmlleqkj.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gqllgntrh.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/ggsmzrkqy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gfclumfvk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/ggmcmzwoi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gbjbfulob.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gfprabqkq.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/ggxtxhity.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gziqvfekr.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gyjhlypdk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzbwneqpg.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gsekhbrwu.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gnntbkjwi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/geihhhjir.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gvtpldzac.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gyssagdcf.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gdedggjqh.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/ggppzvtlu.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gopvkcnrx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gkdxarvpg.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gsxgvlrla.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/grojbooac.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gxvciaskg.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gcxlpkqjp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/grmpwxlrq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gnirymvos.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gjzshigqq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gpiagauej.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gnodvrlor.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gdbztpiht.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gqzkkzabb.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gkzeywaxx.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbauoegqu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gkrotqmhj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gzpbrsylj.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/glyduhowo.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gtwehnoba.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gnjtwxwgd.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gxqncayka.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gxzufbkcs.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gxvqunrrc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gqtiecapd.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/guilyjouk.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gnvgwgpbz.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gpsszorjl.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gxrryegsn.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gufuevuyg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gpmgdhwjb.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gqlfdmcnn.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gdaxryrhq.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/ggjaeymms.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/guzovexrm.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gqqqfahzb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gxbcjtcpl.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gvzrthmoz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gzudllzsb.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gxcnvwpfh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/glvhalkpd.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gvtbhwxcv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/genvahrzu.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/globtdatp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gxtxcbspd.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/ggpodbbjx.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gazkjsdki.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/glwzutnhy.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gypdaxkfn.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gbtryoxha.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/grlkhgfyg.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gzzilpgkl.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gpsmyjbxb.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gmcpvrhve.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/ggnpjxuzo.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gcgktsbsx.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gejrfnlyi.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gsecxluux.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gwrbfscic.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpurcrqqs.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gbqikmmxw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gfopztpjt.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gpaestfrr.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gkkydvpoo.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gencunjan.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/geepjiegz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gfxdhsupj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gyjxidbmh.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/guxmgquck.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/glgfbzeaq.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gamdeaxwb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxzovcrmg.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/geipqfmev.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gxohcdwem.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/glsmyclck.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/ggkvjbgij.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gtivjsvil.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/glgptryar.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/glkxuyedm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gyucrpxoq.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/giupaqitu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/grunjzxvj.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gwxuangdz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gsgrzkbfu.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gzbfpwouc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gjxoxscdw.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gkrirsopa.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gikgwklep.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/grbvzezpk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gcemlikkb.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gndxiejyy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gjcdsfyvs.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxbdlspnc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbfkizjqa.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gcipqadqx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gqeicvbqq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gkwklzbzi.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/ggubnbtcc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gaveakski.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gceewxltm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ghuzmyrpj.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gaswfseav.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gkpqcykou.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gibnedvci.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gqrzwsehh.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gqrqgrmjn.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gijxxsfih.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gbdvzrtpd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gjirdkyis.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gbhtleidb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gktxlrkln.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gcyvuypcr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gvrhhriil.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gfkfnyrvn.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gqhtxyydo.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gdcyemybt.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gqjwsassg.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/grfvguums.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gtioysojc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gwwfjbcku.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gcheyceur.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gajkynrjv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/govxoiqjn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdjsphpjb.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkesrxopw.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gdhajhlug.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gwwaxxlyz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gaaqzmpkv.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gklgjhnwm.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gmskiehlg.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gbnzziggd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gawdzcqzc.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gjkohgnkt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/geivbomfb.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gktbqtdvz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gaylxgyqm.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gphhlnefa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gtyaygqnl.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gactzsbfe.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gdhwchnrl.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gxisvhidm.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gfpqswfty.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gtamqvdsx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/giwyybvoy.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gruqzqdvi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gctdyptdt.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gjruszxze.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gvcqtvdlr.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/geldnwbuz.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gvsqttxgg.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gzqccurlp.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gayeutvhy.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gzikorgiv.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gvydwxfvf.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gabzmgdck.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gufidocfq.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/ggslpsmre.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gwtkfpmus.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gqcsaxcyx.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gshakwzxo.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gaegpidin.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gpctthrgw.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gruwnczkm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gliuxftyt.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gekzjoclu.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gdlzvbnaz.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gvnswjqia.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/ghdzahunu.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gbxfmgfei.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gvfaeedah.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/ggdtjvoad.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gdqhzyeqp.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gsieykczp.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gaxtdhwmz.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gxqblztno.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gpczdolnu.sHtML


<!-- 参考信息 -->