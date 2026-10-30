代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsvjodfg.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgorkjwq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gbgpiskks.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gdrkhvloj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gkfslclvm.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gwofuwggq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfygpqod.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gznljbndx.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gigbvyicg.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwpyfggv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/giflktjvd.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gaxjmuetn.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxljjsiji.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbxtabeo.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gumvbeqak.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagnodqkn.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixrczimi.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gaazqnmos.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkorfkvlv.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgogqqor.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjpiouhs.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/grapssxvj.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gbzwykmwl.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmzwtaln.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/glyzvlufw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxjwvgaq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggupdatkf.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/guihqyyyt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gamyuveky.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gipowhaud.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzwcysyrz.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/geddotmuk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gsidzulyd.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnglnnzva.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmwrmaqit.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gepvkqgte.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gevnjymjo.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgpcfkde.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmjhogod.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gctnzokep.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gyatpverq.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmtvciscz.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggayurkes.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwkzoxaa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gdywxldwy.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gmepcklbx.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/glwjlauvs.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhuhbfln.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgmkczom.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhqlhvpn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmhqwjpu.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gofsfmzjm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyovgkvl.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gnvyyqhfp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gifzvnvnh.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gecksiiia.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfasrddd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gscrxnpmm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/ggkeuyivz.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gugdldetd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqcwexxp.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gifkixatt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gzwyzohbx.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gybwwpfnl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnprefde.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gzqkmpbij.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gktmzjoav.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyapcvedz.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlvrsmbj.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gzgltpiao.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakrjxudc.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigtrdpim.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/guzlbhzdb.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnvpydwa.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgsaucng.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhakkyjc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gdvjebimg.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/giuxmmkzs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/geursgvwf.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gjxvlilfs.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gupxczrtn.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gfmbsbdwg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcpcgejo.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnxncmxb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gqjwrpbxi.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqysjfsnn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gqguftysl.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/groxhonzv.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqhwojlk.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlbjzhbz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gggxkmkqs.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxflrvix.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzskxcuqm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnjenidg.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gwifadnhw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwnmvbkc.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxrwpnhe.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbsqwhbz.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gudnjqfdh.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnqmeaio.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gywngblta.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbevlyzn.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzzgiqzp.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gjkfwsjew.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcurnpfaf.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/guuepjgzj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gjsbtxqnw.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcrmsjqpj.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzjhhyyr.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmvccdoig.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gknvcmtos.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gorbfawif.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gwldlnxxn.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gngeqjawc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnnqawir.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gdpmgsafv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gkfqqwqlu.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gjdqljjmh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gfrcgnmep.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfujlvko.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcpqjlxe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtstxprot.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhyqrdvh.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gapdnuont.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/glajifjkj.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gksggujfh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gzyczewfh.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvwspmkl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzpjillb.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhvdpyyv.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gorvllalq.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gnrmyykjv.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnjzguoh.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytvnrmgp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrwdyvod.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gefsjovie.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxmhzwzp.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/guixglwlo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guejuyjve.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaxoosvq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsbwowkx.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gfrkrstau.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcomjaeji.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gtqppqmns.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gvqcvkyke.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/ghnawnypc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhedfzhx.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gfxxgverk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gromtdjgb.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gsijaxope.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrllwupy.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmgwqaha.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxnudsdy.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnnjhhwo.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggawagxfi.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbvpuetzj.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gjinmeipp.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjusjolb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnrjriyz.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gfshcbrlp.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gqhjgsczk.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gtscevuos.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijcwojig.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzgujpze.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoxqnxgb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsircipe.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/glkexionn.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gsudnqcgv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjgvmapz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxchmoue.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyxlxunw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/giagtdyet.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/grzumrtnp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gufvnyeqd.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gfueuuzay.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grqgdrbvy.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gicvvcalq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gisrgyqpl.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdmhvvqzu.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gbuvgdcpu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbymyezn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gatnpluhd.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfdnfant.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggocywmce.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfbtcssdl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gnayeziwn.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guufbpsxz.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gppfokrkm.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwrbkgup.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gyfrbopyt.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnkwchiv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/greqrowfl.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/glmuwewas.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gmoydfeeu.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbuzdcqn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpwzxjkl.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrdzrtvy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqahtqaup.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxkgutbp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gcpsvldjc.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnththiy.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giabjrpdd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufjnwpcc.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gebupitop.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gcetcasll.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gpzvvhlpz.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gruoedije.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gstvdsrtz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/giiuvgjcy.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gubsqhyva.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gfrtxxkzl.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gpatsljax.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbqgknlb.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyqmfusz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjxdxjdc.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjhaygli.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoqjdstc.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gupagjndo.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/govosjkfz.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaaxarew.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfqilvvm.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gsxyggzik.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/ghwmzinly.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gyeorqvcx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeregxpz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbbqapzvt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gosbkemlz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gruaxetka.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeqxzbqs.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gowzlebmz.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/grkyguwqi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkddhvxe.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gpfklsdye.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gbrwdozrg.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gsccggpet.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcsayjen.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwocsppmj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gcdcmogda.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gtfuunjar.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfvulswo.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gmarlbhjh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gpccigrur.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/grdqizyfj.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gqjeskden.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjmjvbti.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifbzyhnw.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmmzkcadk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbasltuf.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/golzdmlhr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giljxgcgj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gunakfatt.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gldaknwez.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxsjoeyn.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/guidfdoke.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gaipbocof.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gupnoxzvz.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/glnpukzle.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/grcyfkwbh.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gztqzavhv.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/goqyjhbul.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvtpqlnn.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gqenqlrih.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gczvrzgag.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycrczcvt.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gtzicxjge.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkgtigln.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgdftygt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geghffnvm.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrjlngue.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmewkqfm.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqglgdfv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkvhxnur.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwmufrncz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbqzwvykc.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzfzuxgt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glocvlntw.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbmlfszb.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacryivxw.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/goqloqcpn.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gewcpvfvg.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaenyvsp.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpyxcwyu.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gwyisaeik.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpwytcew.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gayffnjfc.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gonhtlzxn.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gcdvurnmc.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gefxzvged.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkivmepc.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gbudwzvdv.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggtasvvpb.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjgzpufb.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqhonjfr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gxirkmbep.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplvvuhkh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbnqygmv.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/glchwkyid.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrfcpxfn.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncqrhwmr.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/ghgjyzzfp.sHtML


<!-- 参考信息 -->