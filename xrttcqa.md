代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggozruaho.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnagsiqb.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/glahtkoen.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghrxdjtlt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpppkkcxp.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gilrtvxjn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwevydkt.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/goozxirwy.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjxmdqhku.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/getnybqvb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/getbgbfyc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqkxrjjc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnhgepwt.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gijeiqdjz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/grdvllsbu.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnyjvbvu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnbniimh.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnagravr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezrlvrfs.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gibdvricj.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwryojcmj.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/geqpuqjit.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gymjbzfyv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gvaldnulb.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrshankv.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gwiatkwgh.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gupnhosvg.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gyregyghr.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxtarjym.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gguazaxpe.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvjrrmgg.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gysyixhmh.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyqwynin.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gonnocxyg.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gymeunoku.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gvqaixduw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/ghhaehmya.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gbapqtzne.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfewvcbc.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gblqkcuzg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gchrczafz.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/guntayevf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczkznfoj.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdizpdxaj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gecjoogpq.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqfxcmql.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gspflhhis.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhrarpjq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gubwczaqf.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gepnyewvu.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grzguuhpc.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gopjypzlq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gbqnugdgl.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gofhvisua.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfltjcgx.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/godjxhryp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoedkaih.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbsohhay.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuycyise.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gqhfnflgy.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gyliltxkj.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtbyoiqzv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/ggyuxutri.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gygknwegf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gafoicqxs.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gwewqvypl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gahvgpuik.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/grssbukcp.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gozkkexio.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gevsivfeh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gycajbvrt.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gkrrmytiu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjaxqhqn.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjdxkwoy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdrmwfhy.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/grwhyghxh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/guxfbkwvc.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/glegnlxfs.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyqmkcnp.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgdixxmf.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gsecvtcyn.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvhhpxuw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsyiugccf.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifgvuhvz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gecfzbvcv.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gttuvskfw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gvcphljgy.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gfrifrupi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyamwvrx.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gbdpusdkb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzyxrpry.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwivywdn.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gpauufjle.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsogiprfr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmqmfsgha.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gafhsmrcx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtanrqlwc.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goxmzhnlb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtffvhym.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gkxobkxli.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/ghlfkkaeh.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvponqjd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggwushblc.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/glkxxyihz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkpebfxy.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gcpccuqzl.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/ggztrtvjx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmtqnbgoz.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrtuqrjb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gencvycqq.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfjciyya.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmjonpwj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfrvnrmqy.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlftgwuc.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gqplbcdiu.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlybfpap.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/glagjfrdo.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gykjztelh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gxapztosf.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/geetuwalj.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/goqhzocft.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdounbdxg.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gukqkkldz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdwvysaw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gheltfrht.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gulqhvtxc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqcyvkxf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/geaclnzjh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfyjbkjd.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gqvdpoygr.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaxjdgud.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvfdebnh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gowceioai.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzlvbykb.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gijfbhusi.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gslkjenyn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gbukyoreu.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkhjzawd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gqfwagjmj.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gsjtpslmh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gjjysgtpv.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftfsbuvm.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoqutuie.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtebrpkce.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/guczrzwtm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gobljmbvk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/giqamempd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliuvnfob.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/ggnxnlbrg.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavokemec.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/guafuvwdl.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/giyxnyglb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/govskioij.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdohkowah.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizhudmvr.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gwvlrunir.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/ggiiozoqq.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidtjkvqr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/grlwrxwzh.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqeabahv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdkfswvd.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkallpel.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaobzdfqq.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrwqjllk.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnifwvjrb.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefjehqnn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdiibfdm.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzljlied.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpkqqsmm.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdylxnia.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnpcrhem.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvcpunlv.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/girulifod.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdfbikuy.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gbtudcxoe.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzfqdthka.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtroqtjr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzpwcuxpt.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gekrwpswh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/guneqwdvf.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/ghvwbouvh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/giwdsqykd.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gwcmlymsi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsmjvvdme.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfdciaam.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwakodkhs.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqlowxbq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gazptknrd.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbyhruln.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggadqplan.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbwzlncz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtmvhcuc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/glrmkskyq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gaotagipc.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gbciqzmly.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gubjwhwlo.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpugfmlef.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gslacshvq.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmebdvqpm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqpzkhwp.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gavewpymc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqxkuhdj.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqqdzgun.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbwzamniz.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gtpchvkho.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrqqoetk.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbivyuwk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcloggry.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gsfafnmjn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyyjpvsd.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqhvywvkh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gthpxxdjf.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghkcmyqeq.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmzblakyc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gdeviwxuk.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/girkbqhvi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gqsmvccgc.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gsdqxddwk.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzxajoci.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gcdsxehkr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxmtwskgn.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gaarfryok.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjanpsodu.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuqmvagi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghesqicoo.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gdukuchox.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/guwdcmxmv.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gevufiguk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gatbscyir.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/guxwoxuph.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/grdqplndu.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/glqkjlotx.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gkrbptqsf.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gogynvjoz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdesluvyv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpkbsqzg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/geiejbuxz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gypkhexry.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/graaikkac.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsylxucxe.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ggmwaqdss.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxclgwull.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqjogcqz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxgocqov.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ggobekzjv.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlbvbxbk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/guokdbnzj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkofdzlc.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gmqywxlxp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gzkmjkwci.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbgunefn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpqipsuv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaozbnli.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gdqcetsup.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gfarvssvj.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gpwikkjhu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjahlyfw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebbjjfth.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdixomztj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuuyjizg.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gntvnxzdy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gognrgkcr.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwrhhgvg.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gkbwztwlc.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmpgqtlk.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtappcilv.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggfztxxzo.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlhcivau.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifhkcjdg.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gmnkwyvax.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdumdqntx.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjscqqvod.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqqhunds.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrbptzue.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/guixgwuxg.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gzjeforqy.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gylspkqqt.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gqbwagile.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvqrzcmh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvqerlhq.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gjvbjnutv.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxqsjhjc.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gudtntydh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdzszjoh.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwqpfftig.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gntumtkfq.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gqckhyejr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/glnettgvw.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gwqbiglws.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gsxzftfoh.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvjqciik.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjorhlgke.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gdgaoqjdk.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gocsiuzrp.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ggkpuqlwc.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhppwurm.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gmlqxgaij.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhtpkqpe.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/goiuccbvi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvyqxzbb.sHtML


<!-- 参考信息 -->