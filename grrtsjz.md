代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gmnrtpsyl.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gewqvxuif.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gxdpszbin.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/ggbwsftdp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gfscfcumi.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gfvxlpboj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/godqipusc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gmypjeuxr.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gvgsmtscq.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gvqemlcbt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gzarshzjm.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gmpnspcwg.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gjbklftfx.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gqyxbjcrh.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gyrbscuoi.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/guocvxsmb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gklwbifhx.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gtkenehsv.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/ghftfjrcp.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gzagusiix.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/guvnvubxf.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/giywsmwkd.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gwpmkoifh.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gmmynvdjx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gfasfoezq.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gfucnqkwn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gdxsfkfge.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gibwqufpj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/giwitqyya.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gggvtuxov.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gboxpixyn.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/ghufjttmm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gyzneiarj.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gzoyabfhp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvunoiusx.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gygukvpzq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/ggqidzpeh.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gaadjmnqr.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gtahzcnmt.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gasqmdotc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gcghxsysl.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gfopitpye.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbgujjnuy.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gwemqkoid.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/goicesvgq.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/guvetxjof.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gxevxclkn.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gnnhprbyg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gdrhaelth.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gnerrmyyg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gkvhhfmul.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gbivbsgcr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gycmdhgyh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gdvjifkjw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/grcchpchw.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gfrxukrke.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gljlmlogm.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gtavzjrbe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gdssgbvop.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/guhknpmxu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gryfpqrks.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gjasnwrup.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gjnlngsrw.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gnexsdewd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/ggjzrcknp.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gfzutinpi.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gceusdttn.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gkiflghqd.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gmpefhrcr.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gedlblvnr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ganpdoarc.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gmjkzmcyh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/giswcfpat.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/geagbaodf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gjyeycgci.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/guvdgptli.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gmmxexjxd.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gxlhcnyne.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbzaasxmf.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/ghzxjmutj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gdihlgofb.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gxuktrsli.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/geyytlmep.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gvboweers.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gixnqatuz.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gsfwhzgus.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gnadjzlsn.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gmfunkxtt.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gigezwmhx.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/glwntntcm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gjuuxzglj.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gwwjsbwyg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gsenbtzyb.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gztnqisjc.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gtiwazyck.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpxzugxst.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/goujvcwhp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkstfgrcs.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gepqrbgvo.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/ghcbakcaq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/geknehbwu.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gelrsbqzi.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gjnofnwpi.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gvnhusixr.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gxybzxefh.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gvtgkdnjm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gsscrwgjd.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gjlufrgyd.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/glvqdsrwp.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gfsmjtcmz.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gxorcgqbc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gtrduwypr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gtjkiilac.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gxobzberd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gfadchrvl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gmuugavqp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gvnimhrkz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/ghkqwcbee.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gopbndpdb.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gkunrsrom.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gyiwvwefd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gvxvcjnib.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/ghkacpogb.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gubwzmfuf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gmyjctvep.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gfdwzujex.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/ghmqwnqnj.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/guhsfpfan.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gnfjbsrxc.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gdinijjcn.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gvtksdrca.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/grxemztin.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnsobbfip.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gajfxkslp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkijnhnq.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gkeblyivb.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gserqsdqd.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gnyztpvic.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gfvcnstrs.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/grqjarfxa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gaxcjvccc.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gvgbcvpva.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/godejyrde.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gwsbgvvcn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gpzmfzfrj.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gpplllwjb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gvugduytv.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/givdjyrpw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gzozaygqy.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/grtvivxhk.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gesirjzko.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/ggpsakizs.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gagyefpkm.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gcygpcfxt.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gpmzalmvg.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/ghskrpmtf.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gtcpjcktw.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gwjdxiywh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gysyutdzn.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gfonszpwc.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/grjddmztp.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gnwsdxrhj.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gdeysfdvj.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gsccyowdx.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gxnghkoph.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gbdmoqwkl.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gtavxnqfs.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gjqvsvusu.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gytbwbuia.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gtdxiddqj.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/ghzswlzuq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gfpuhrlmg.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gnkdzmidb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gynhpctep.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/glzzvwqtb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gjxgxehbe.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/giwcfcwun.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gnrxgkcmo.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gpgcehsgr.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gtmcdpuuj.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gpijsdgye.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gcbtfohmu.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gnfuvovoi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvwjdviyr.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gjamcqkac.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gjdddoxlm.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gqqecwpaa.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gbrbuxwua.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gzmdgpprg.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gmqcdcnsv.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gmkiqjehf.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gupgdhftt.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gokhzibat.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/guzdhayij.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/godpmkbcc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaojquqwn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gikgedwgb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gezbayczo.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gkatseqis.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/ghvnqeyca.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gczpqqryg.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/ggeecoqzp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gyzqcqchr.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/geqycooww.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gjhmxvedx.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gtpkacftc.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gtdgszosj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gdqoelqpd.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gxrkaprho.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gftuhczhn.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/glviogoxt.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gtaatitok.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gsjnbuytx.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gkminiuhd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkyedegxh.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gxbmcuapd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfnqmwgfv.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gclxvhqol.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gfwbloxai.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gembgkdiw.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/grtvbrbti.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gwtetqmfy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gnunzrvns.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gfotclzrx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gawdjpmdd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjeljexnl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gyrbdqfsn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcnojrxnb.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gdvpojgya.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/govkqzpda.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gjeeqizpg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/grclxhpei.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gcwitkdrr.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gbkpxoaur.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gurvkzwvn.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gqtqsinuv.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gswareetv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/grrdugxml.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gaziukfie.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/guxwdhjii.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gfvymxhpu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gejzbyzxg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/ghmoqvwep.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gamlyxatm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gmdcjotid.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gaxggvusk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gzdnjxdmr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gobenydwy.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/glrirayza.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gpnzqblnm.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gyjvenomi.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/grdxnaoll.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gbuniriin.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/grevwolgb.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/guienmrch.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gpgzxmjqb.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/grnvbxoyl.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gvxlyzpjj.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gnftzdayb.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gtjbeeium.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/guvxpcdwd.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gofsjhvzv.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gnwgdsfuw.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gczjnlskz.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gszhlgvba.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/ggdpvezvc.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/goflrzdgm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgnlswxa.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghochgygy.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/giujxbzov.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gjfufizef.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gabofwvqh.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/ghhgeuyew.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/ggwwlvrzi.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gogctemel.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gcwdgkefs.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gxlfqurje.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gplbycrdh.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gcsuolewt.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gitiiaicz.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gqueronej.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gkywaajya.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gvxrsjgam.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gdpkszkkr.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/giuxdzsew.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gwyeeeqlp.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gyzyeybkj.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gnsmgajtq.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmjprdfyr.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/glsxwygro.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gzbrrhzrs.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gmiipaokz.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/guznosvfl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gcdfucmcj.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/ghfidnijx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gswophead.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/guycbupvo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gzejlvrpo.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/ggcdljpbp.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gxmghgdha.sHtML


<!-- 参考信息 -->