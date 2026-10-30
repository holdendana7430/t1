代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/grspplbcy.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gfupmlpry.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gjwifnmgq.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gfmypcgjy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gntaqogil.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/getkvcjvp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gghqilbgw.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gnovzyyay.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gyjzlgxrh.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gmjinokpp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gyjjdniqp.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gpwtlahqc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gfutmxnkm.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gxocrkzub.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gafvfymex.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gotcbueed.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/galysatcu.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gjxigbqsk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gxkgeerov.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/grdsifjpz.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gmviswpkt.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gycadvwan.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gcpmpqufb.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gutgzfijs.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/ggtgvcnvj.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gvvdglhyq.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/ghhnospzo.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gatubtdcd.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gyhywqypj.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gezgyihxe.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gxgtonvue.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gkegdtnvg.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gnjevmvxl.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/geztgwdra.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gcomsfeys.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gscpflhpo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gifofqyio.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gcxpigdbb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/glyymudvv.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gsxqbhpos.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gdgnihzcd.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gmhvijohq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/ghisbgvfr.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gpqpgdnyo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gwrwqlbyy.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gqtvkomrj.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gqznyzdjt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gxlkhgnui.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gudgtpwqs.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gnbbemqou.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gbydlluzz.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/ggewprjlo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/grwbsyhwf.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gwratnyfm.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gtqxfobea.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/grntlcxdf.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gnfzshvxz.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/grnyurbhi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gocgwjwbi.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gxyoyvekt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gmffxbmmi.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gtrixacts.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gckdbyidp.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gbiyaprua.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gvatrsjrr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/glrnqswqt.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gwkrztzll.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gzbnkljje.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gfumzuila.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/ghggcvmfq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gxvelnfav.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gqmmbajbx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gdavuedlf.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gqmppmeab.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/garqytmkw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gtrehkipl.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gmdmxcxzb.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gzqmjhgah.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/givrzyrke.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gccxoywia.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gqiyvgamr.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gzehfhaze.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gfqgcdbbs.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/ghzfkksyd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gsocwcuel.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gbzpsnogh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gkthmcenk.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gnzsrmnzp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/goywnhcyz.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/guveytztt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gkwgxwhzr.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gqagwplol.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gallyddyx.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gzupkzpnq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/ghzvgogvx.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gegntxdgr.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gneqzupts.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gsvydkrao.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gojqgffwo.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/giekusctc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gpfjtpjzm.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/grkzinkum.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gldwuoylx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnhnlmnkw.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gwoyfgyze.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guzlelwcc.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdfbhltmf.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/ggdzpaxsh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gsxbozehl.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gszuxjean.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gxpotvubo.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gdvmwjtop.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gocdawehh.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gbvsbwfcc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/grovfotdq.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/grmsvjacv.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gcbvwzigk.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gmhdalulq.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gyqeurjky.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gmvnlcatj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/goqlexdbr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gvfzfdcrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gjtzujfcq.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gcmpjoggr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gvxzjmgae.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/ghyoxxhll.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gqfekbseb.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzdkzcqdi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gkoyozbzn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gshdgurbk.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gtpfsrmln.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gdzwbinlb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gbsrhnsbr.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gdcgrvbmh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gwaoykoya.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gvfumktqe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gkkvyrfsy.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/grszlnvdz.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gojznmuzb.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gdnfberew.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gqjgnxipi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ghuvjbnjl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gumibhfvh.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gvvforurq.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gqpdhowae.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gnzztazzk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ghiuwmqpl.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gqgaercrx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gbpyatrvp.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gzfxgdnbx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gbponmbgt.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gvzkkfxfa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gksnmizqa.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gqasfanpa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gulutzwzm.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gsdbkfwmm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gmowzvcsu.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gueovwfsc.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gpytnxyly.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gdaohgdat.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gqwrgaxkq.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gwakgkuzm.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gjojdlrte.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/ghmqsqjwt.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gsbkgycko.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gxjfkrlve.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/grmcmjxbz.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gfifgekxa.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gxnroxjut.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/grhrcipdt.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gjnegcqsk.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gpxluqsgu.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gbzzgjbpc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gkrhlkaim.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbpudkdjw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gllrclyoi.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/ggqhmcfzp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gzkibarti.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gmulqavdx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gnomadyul.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gvgdpjtpp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gmeupkski.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gyhrbbnqg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gamwyfhgo.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gkwvzsfxp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gcouoaiae.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gcbzwkack.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gzqqamppt.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gbmpcuvmz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gyhlzcqsa.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gcmurmpzy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gspkdfojd.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gwjhdnnal.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gajwenrfs.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gmeyxgaek.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gfptmbgak.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gzkivhqvm.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/goabydxsk.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gedqnxhio.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gwgxhwhmo.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gajitwuhv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/ggxmuafmy.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gsxeopoju.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gvfgomywi.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gixjjdufc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gzvzqhsdw.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gdvrugxyi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gwppqnygg.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gwzfchryw.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gbueckino.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/goggtgxre.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gfubqnexg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gaviogcbi.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gxaxpaynu.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/guueogrru.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/giglxlynk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gvxzjpzxj.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gudwaahgc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gvjxjjlli.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gazenizbi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gpxlofqbp.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gofdvnfsb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gmqquuuvd.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gsokyfurf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gfdatvzye.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/glgawpkvy.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gdbvzyyen.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gonunsdrc.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/grtmfbvon.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gxavageyx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gxcuhzqnr.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gnvvzmqqo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gdxqfhfdd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gworpmzjc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/ggpppcbly.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grsijlsvp.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzwncmfon.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gsjebqhpp.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gcexkjwwp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/glikubcuz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gjmnsqluz.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gkqhgldih.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gdberbsek.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gsgxyejou.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gcekskaoc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/geflcoeec.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gqycgktje.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/grhtfxies.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gynbwzqvj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gqwzlhdts.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gbuzedbue.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gwbczkgmt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/glabokbba.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gpgaihgha.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gqjgcnxxb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gaopwthoi.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gbamqsuka.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/grfdqirwd.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/goysdftax.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gpugbohua.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gvzoaqizx.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gqrcsayts.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gczwmtxfr.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gyuwweojj.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gozysexwl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gfdtcbssm.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfxhklmrd.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gjvefgpzi.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gkfosnbyg.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gugotmcdz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ghgfyiocx.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gcfgzsywf.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gzsciehnz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gubmwjgva.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/guaegnptt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gjmjzclgo.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gbgeuaohs.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/goohlbblj.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gdhmwixyi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/ghqziuwuh.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gztbynboe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gaklxlsyq.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gajjufaah.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gzrhzeeok.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gyagfrgin.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gowrxltgv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gwsvvlowo.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gfqcnczel.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/ggyzncbdo.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/glynjbcfv.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/ggcgpxsos.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gaducddtc.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gyobubkzo.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gpsjqfgee.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gpmbpdffa.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gseucoaxu.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ggtwawriq.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gicelbljc.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/ghijkwkqq.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/goxbslxii.sHtML


<!-- 参考信息 -->