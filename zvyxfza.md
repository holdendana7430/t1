代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqorpgmyi.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/ghbxtlnqd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/guywvmsix.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/ghubxxnyt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwroqdyjn.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/ggloorzdz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/ggldptdpd.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnqtfsrb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghadaxtvo.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gqnfuxeru.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszywotax.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gozjrmbim.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdvsisbo.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmmgpyop.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/guzjijope.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/grvrhhtex.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gjtqgnqmt.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblbuudxl.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/grglogfdv.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/guuolxiys.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ggxtuxcaj.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkxnxjwj.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvkqmeyc.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnsfmxxh.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ghkvydokf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkuhxfhg.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxbpakwb.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqnfduov.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/grrikrtht.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gdoxfgkmt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/goqrhcwrp.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmotgbejy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmldomsxv.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gbnrpambf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghjjpaprz.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyurydpov.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gegalooqe.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gzdpcvbxa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmbsjlos.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/guqrdbpga.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/guitqzkwo.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaidyqrv.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsloxqknf.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gqpbprssc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxfortqi.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gstgcivno.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gduyjwbwd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzgevtyi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gdwyfiguv.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/groxgqnfu.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gitecbdpw.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/grksfqvje.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/grcdsbyct.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdnzkcvu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gziyyrfii.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcmzgicd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/guugfwgub.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gouhtdaas.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gujiqztue.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gnwgrpflm.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqnopety.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbqprylf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/ghacromun.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giokesxfo.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gscigsrbt.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzybzikji.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gakzlapzd.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjxdnsma.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gajinrrwe.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgvbptbm.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gcmcpcimz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnlaeild.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gesoozsfo.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gjakhumdx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjibajcn.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgoujgmh.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/ghvsluska.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gjxsyrbbp.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gxeeyadyc.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gejhgokjh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmiebxoe.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/grfkebelh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnfdnhir.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjwbutuii.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gdpouycjw.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gsznevbqj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gngjtjrcc.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcploipjs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaolhhbez.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmddamquh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/grrzypfny.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/giwneduro.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gbazlryze.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkkountz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzuacqpi.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyngfexhq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gojuapcmf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gecghwmnx.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmjrrocy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcaocclap.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpqoqzyc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyttobqef.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/guemjufck.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhepidhc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggcagoocp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhziqwqx.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gxfkjgywx.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gopkbllfc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoizvtwl.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/glfgraivw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gmnrnslrl.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ggfbnhftb.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gutzuukvu.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgdhnhvw.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcnysonz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gydgqaqkq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gbbxyleeb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxtlucwr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmdrvkki.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gsmeylliq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgwqrrxd.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoyaqeon.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gbclqhiuo.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvacbuifn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhmdrcjy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfszqmhxq.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gvwgvivqc.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhvzaboq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsutcqhdt.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbrlcpcs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxipnfyli.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifazagtj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gplitovzz.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/goaqcgnjv.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gbrmfoydz.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gkepuyvpt.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvnotdpt.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvyquxkc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gurpqhimz.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwurnwdys.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gmjwmifak.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcihqvoe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gtfeoshod.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gigkltfgl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gjcyqtmcr.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbzubnrt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzlrgrwr.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/ggxagpjfc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxebwjnlf.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gkohbbzdf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/goiasbtbf.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/ggknmqhyv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtlqwcfd.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gfygiofsj.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnblymjh.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzluizrv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyxargst.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsflnybu.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gwyqfzayj.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gojtsnnsq.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gqjzakfqu.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjquhzios.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gapsllchc.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqunqoqw.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/golskegex.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtmgpued.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gzudcxzrz.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzzqfwlzf.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/givxsfkhn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gznmpfktx.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gxsobrfkp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/guguujdzd.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gmtwytjkr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonpwgltn.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/galpjcojn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcwdazxdq.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/grwvfbazj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvppefvl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlrwyfjn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsxdcksu.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaflcgrsq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grxccwynx.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyuwuvzf.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/guwtrwjlx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjqjgbce.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gsjwdeftz.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyodepwf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gqcgksxar.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggcqomqhe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrzyderf.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakcldgjz.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gcbglskni.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gfdiossfx.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzebfctpi.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiwqmakq.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/grjamyaei.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujvtfffs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gaamscubp.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gklgweyxc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwevqyfa.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/geekznmut.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/giwugztqb.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzmprpxbf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdlhaakw.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdahfsld.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gotvcfelt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/glaidrexi.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/ghejdtiin.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojanthfw.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsvrthgd.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/govfeboro.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqjcnfvk.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gipvdmnlk.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvupyhair.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghckntnye.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gthvattzm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gbxbudjbn.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvtwuduz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gqctrnfjk.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhjbuyxi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjavdcvou.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/ghkdtmopp.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnawczdpj.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/getvnjgyn.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gcqjkvghn.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesdxotvp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwohtvdya.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gizafbgje.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gbsawxqqo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzjgknkt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwswixvdq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guvopkbmj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gimordvwa.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/goqlckriq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpjvnjgi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsbyuamq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/guwfxuegv.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwfiiiki.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluofeicl.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gwrodwkib.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgdkmspn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaakagszm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsdcmtdg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmspavzm.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gextsitss.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gshkiednh.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gowdarccp.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/glhampghm.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/goazzycbb.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpscskdea.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gmwenvzme.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gapwwcsmk.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gbhzaspib.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmycstoj.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbmfjqdp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnojhwoo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvljivwod.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwhohzdhe.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpflbaoe.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goktzixso.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gwcyiibil.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/glowsnsvj.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfdisjjcv.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpqdsruc.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gxyapvljk.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gucgbdldc.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gsdeqmsly.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptmjksaf.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gaozzszqg.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gioutkvqi.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrzmhuef.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfafmbttn.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcaphhja.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gscywhsvb.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwqmozeq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnwmhprop.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcznwtabk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/giuhtarte.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gnxvgrnua.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gopmlysbp.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqibhyhmy.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gianhkhqz.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gfjwijksy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzinlovld.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/glavlkpoi.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblbscopr.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/goibvznhg.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrgfmplc.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjufzecc.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gppotzsli.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpggxmrea.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzpzzhqm.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqducrbwi.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gngdzlhwz.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyinkerhe.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmuxaike.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gbfuiokcx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkcekzvf.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/glmqjqkkb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxhfjobe.sHtML


<!-- 参考信息 -->