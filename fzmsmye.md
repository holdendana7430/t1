代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gopaoagit.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gyrodgarf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwizlhpbl.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmbybzkl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdasyjgs.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gvzslxotd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gvykujrtv.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpjlaylg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmruptqk.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gvfimmmsm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdggefix.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/givdhtwem.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnkrpeqv.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gifsdhjby.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekokbsdo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grncmtlee.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhvsuqfw.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmnetxtc.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpboxvhjf.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gspcqpthg.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/grmykqfgd.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gktqzxhhy.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhzgdlsx.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcwymuvbd.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gpbawjmub.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gicevvfgk.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ggclibdqq.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvwkqxcj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/grtklwuxn.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gdolpxhkw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/geifpvlqm.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/goujdpmqk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavqtheju.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gvxcjpmjc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvlhutqel.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gemxxazwi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqsosfxx.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gcaziyxqv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grpfyczho.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gawbyidtp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmnqrfzt.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/grszntyeh.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgtjylbq.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/grgeprpxh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gkxsegzkk.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjoswtyi.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoegmvqj.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlpfrzam.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgshloyu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqriyzcio.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/grsresjax.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgyzeipt.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gtndbhsqf.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaejpityg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gzbudgsza.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gmgustfyw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkbwropv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gybqfkihx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gvmytlacv.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaiviodj.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmophcyz.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfskrjfg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqtpakrs.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gavqmypvs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmixfhqrk.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gporonlin.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyydswgxj.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/grzquylql.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpoabktu.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvfatsak.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizfcqjdt.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gwbkqnaay.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/ggyviczmk.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbzqcsba.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonuwkyan.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gynblyuwi.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gbcfxktub.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gucpnbwgh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gvxnazxjt.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gfteplroh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuamnppr.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcprvxwp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikovqfyl.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gyqqjmkas.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/geqboosop.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gsdhgmobl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvcxxrbbd.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzcwephks.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiyqvjne.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdzdlixj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gcunlhlna.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmrxxswh.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gahravbyr.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwevvhrct.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtljsraz.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gfjzvdruf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjldmklzy.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gcfwlmrtu.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbraririy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghrshxiaa.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gbvuvjyku.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnsythynt.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvtrxkmq.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gsoucnhat.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvtcbrzg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjyqrykj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjmckwfq.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gkucrzqui.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqynrcrdg.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqmfxysu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gggmrqynn.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/ggtwyytsb.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpxkucygj.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gymrvtovt.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvxwdhzq.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/glckwpozh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkvitttt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoyhvziz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/greprkzun.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gqagvxqtz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gynkqwnxz.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/guxmteaga.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gakbluzmo.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guvdmughw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gwpdgqumm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/giozebxau.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/glhdzpkep.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfohuopst.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzbayxak.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/ggfhesvne.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gkdgnugad.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gadpsquue.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/glvcsafny.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmfqbrvkd.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqylazlm.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gthwfqzsw.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbywfwpxm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvacolaei.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbmtjutl.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghonpguvo.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gmczgfoop.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gyjzvagyv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqdmjtyd.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gfnezasio.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goajpgbtz.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrinrtwq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gwrbvknox.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepoagdna.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gsuxhiwqy.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoivnyek.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnjpufxa.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gnatqhngl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwuuhefh.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gwkpgpxkg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnmiskcm.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjiesujq.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gmfhdwelg.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygyyngqx.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gpznfhnse.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmicauruo.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabjrmchy.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gezndfkcx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gfolapevj.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gfirfsjxz.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/ginjnkmdu.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtwqbvje.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/ghucxikmq.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghugjpdgl.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gumszbsoy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtomjbtkg.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gtqnynysg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gngllrlci.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvqenduw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaezfrhps.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gexkaqkop.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjisovcsx.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/ghhtjhwmo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxrovupj.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gucupdfau.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcinqqoe.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmdddngd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvsfmvlp.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfvwropu.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gljlilhnu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gucbovawd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gzrhdyrha.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupszrkbv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gekhphrih.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvxzkelo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gldeoilyj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiacvuyf.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gdgvzbech.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/geeuvyfpz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixtzobfx.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gcvetotfb.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkbjzqwh.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gflxxloln.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/goqtwbbwx.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gjvwfxrck.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjebxjwoh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gcnvftccq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwwruqsc.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgcxppvf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtducyrmh.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxiekdypc.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glvcybjnl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvhamtft.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjefqkja.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gnxlspcvm.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gndlemihy.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gxefhdvbs.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gughwirgh.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gywhwkddh.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/ghhkjwfbj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/guhsqyyxl.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/giedbcodi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdnyjmetg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbgbquid.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gjiuibtrv.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbncakhf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gczgjvsmh.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnsegkfq.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcycyqfmd.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gbyxrshqb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaudynau.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gidxgxpqp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gjdjhaayx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gekogndke.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gmwkxwscg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghigeggsy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwegsqvb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwqonjiwa.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnjfcwyt.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gvfgizfde.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/goewnkvza.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gcrfyrwsj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gpmissbvc.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gyymqrosa.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqynlsak.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyvrmqrg.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gcxvxwwmr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/guodozvzl.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdlbrfoj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsigkwap.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gnhnbylez.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwuesapct.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gnudayexk.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gtukdzyzb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadciperj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gtktfalhk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gurusnzse.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gcqkqraii.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdrdbyhs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmwjupyu.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqrrzwpl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmerilpd.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gkooetmmq.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gerfibing.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gdnnhrjpo.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkjsyucf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpqtksuy.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlunhymp.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gidmaudik.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gceowaqnm.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gvwutvjsq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkenquxmz.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeqdcwge.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/goqltxwfj.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gizprowgh.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmiszhcw.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gydxxvfho.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gdknmelsz.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtitfhjrx.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gaxffgpcp.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gehtkgwcj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gfzqholom.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gczbiokix.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbysuszh.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gofmqnhtz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/grpsteary.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gjveyljdr.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gidwhtujd.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/grdjgwkgq.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gdnayyfjo.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqvjbuow.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkudaqqwx.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gkqbfrrvq.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/ggzheqvog.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/ghwhfdnly.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/glntlloni.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlnhnyte.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzlhnsxi.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmahatgdq.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gojnpydgm.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwrvjfrty.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpezwtqb.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggioggirx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gtowmdqwi.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gwdasyjry.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gnszwlkyv.sHtML


<!-- 参考信息 -->