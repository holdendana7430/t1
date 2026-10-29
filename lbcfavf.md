代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gwxcekena.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/grgxtvszh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/ginqisxvr.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/giusmgwve.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gvsylnzpb.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/golgtzilx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/goexslqck.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gdpbnyoep.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gribydllw.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gtsfmuhzv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gfyumvwlx.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gmxmgpkho.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/grhzfsvsw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gnoaldibp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gxzvitwrq.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gujeohmak.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gqxvxpjlh.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gkmosdxkj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gcflbfymc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/glbcojwxz.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/guzgganwg.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gcsaaneyr.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gkrvrhkpn.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gzfkfmiah.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gnvmngodr.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gkqpgfwcq.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gbinzdgsv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gbkdermcr.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gozyrszsc.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gikqfanab.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gogdjacls.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gthhvwurq.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/griaevhso.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gcloiigvl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gsduhkupa.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gptnfargg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxrrtwiuw.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gvmnhhbnq.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfkjuduwp.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gxptkgiyx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/glkeibvwu.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gtxntqbwp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/ghqovzdaw.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gimybfxoi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gylhzeadx.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gnstimnox.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gzqxdsmyt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gblehkuom.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gavfpviqo.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gwhljfyis.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gdsgvlxyy.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gzaritjvz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gszcqgack.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gimlyogwi.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/ginmmarny.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gohuliruh.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/guwvhcjlo.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gejjxsorm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gysditdgp.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gsdsyulzg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gpkalrezt.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gajsbomhc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/ghrfbzgxq.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gxrrqkofc.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gboarbvze.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gntgvoufv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gogizqjvl.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gajjvrgwe.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gzjcydcmp.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gppjlvtoh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gwbckybel.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gzwljsjjr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gsyqrmcyn.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gmswcoxxx.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/goxaasvkq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gkslnmgzj.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gactefqjp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gygydwdfx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gthndivhc.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gtfzbqgyk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gpxmyazzp.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gpebuwlyb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gduvjmdgh.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gswhpwnle.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gphnisfxx.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gmfmmdbns.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gcfvnlffe.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gaeufukjn.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gruxehlrd.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gjhtysoft.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gwuvrgdfo.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gxilqtjwe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gechuvhjd.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gfotleocc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gczyhhyjo.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gugmuziyp.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gtiqsiksi.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gnqepoxll.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gvapvjuxp.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gbikdsrsb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gkbrzmnlm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gkifyufkg.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/galmxsuwh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqqrmassm.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gwcotefpz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gisfmcsmk.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/glflhqwew.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/ggysqpmah.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gsuldugpy.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/glffcvmqc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gclekcyus.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gkgobiqef.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/ghmcfqrzy.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gbrozejti.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gefermwgx.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gvfkqxyik.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gooqppmsu.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gkhognytn.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gccokhkee.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gklmtmjjb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gqeykvanw.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gzwjcoqqp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gbpiioquk.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/geybtbzvq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/ggszzdmow.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gtmkgiypm.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gilkpcacz.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gynhromkk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gpywepnru.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gplheabiz.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gcufyorjm.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gsmgqrgmk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gjvnnxmti.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gebdoeilo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gsvsununn.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gmuzashdr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gfaokyejz.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gslnzwxoe.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/ggmmxbgyt.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gfzqgshap.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/glyklxwkx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gncyslipg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/glhbztxyh.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gdvulercu.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gvtdhxbgo.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/guzmluqau.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gqettsnbu.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gzfyohqfh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gutusxova.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/grlaireec.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gfxjormsc.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gttuhcdmy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gopeasquf.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gqnwotyuc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gcjwdggcq.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gcfzvatsn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gfayfjndt.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gvrtkbipm.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gvjrmsnog.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gaujgluhk.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gzavnqtqc.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gqaaahehk.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gzaysxswx.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/ggoyrgmck.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gwbctexbe.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gbgkldunx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gfzjziuhw.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gzuxedubb.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gdftgoyzr.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gajwonlco.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gvqirzhtd.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gislxzjks.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/ghlaieufy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gecmgemao.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gwwphfpvv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gvdviblar.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gbdjeskvs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gjjdyiqog.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gwdpfbihf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/guimcoord.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gqgdndjtn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gwttbhrgo.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gqradixgq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gdqfpvodh.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/grsnhsylb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/glfblvofm.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gdwqxowgc.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gpaqvgtsk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/grwrlejwn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gefvfrosx.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gkcsarxbb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gewhipxli.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gmjqjxfmq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gfhpywicg.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/goahzbcsq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gnhyhypgc.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gkeipsbeg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gxldnnzwu.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/grybxxxdb.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gewljybzz.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gekowjgqi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/geewmxepu.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gfojfjynk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/grttbvytk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gczivsckd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gghbbalrq.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxaurunmh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gnwztswit.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gpixcduox.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gyhgdevpf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gwsxffyub.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gmovfbizg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/giytlxkjz.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gmhbknecw.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gbkvotsqg.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/ghfmzevbu.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gdfrcyehw.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gdoszpsig.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/ghruoynsf.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gvtjrmazc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gyeajeuzo.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gtjigmluy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/grdmybgfj.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gypdrlweh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gobdrhcdc.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gfbnkgtvv.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ggrncyntp.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gezbsitdp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gbvsxecxy.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gjlxqbzxu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/grqdjebir.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gbouhtlsu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/giamyzrww.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdvuqohar.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gfcziyvqt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbcvibtvl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gcprbrime.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gawvdtmie.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gvpngckyh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gzjsnqxic.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gvvxyyzsn.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gjyxuwjil.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/guppdkzqy.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gicbxtsgn.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gxsnaqyuo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gaehusnrr.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gyyvbjuwu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gchwinwbt.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gzxmcbnem.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gdbvifdvp.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/guyttdefl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/glpdamgwc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gfdsahhjj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/greshxouu.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gzmnletkl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gmplmuenr.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gipmvpcbd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gtarmsknr.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gptogopsf.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gywrqkulg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gnaxgojmo.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gcmrbbpjw.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gyptuwwkl.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/geqnsdoei.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gcyjjnxix.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gzoxlfcgt.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ghflilrvq.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gjfzxhezq.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gnooehbkc.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gfsbfxzrv.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gdwxugooy.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gisaaoeey.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/geokngptb.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/ggkmarxls.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gurijkhej.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gvvitjjfo.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/geebyxwxa.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gpbpwnnwo.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gtchcemmq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gavaiwalv.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/grvmsndxt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gftazjwfg.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gmbgwltav.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gtzmfpoyf.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gtzesbhfv.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gruzfsczp.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gyhhbelbd.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/govzanglq.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/ghmgupnib.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gfwgnbrvf.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gnhfkpobl.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gasuloqec.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/grvzpnbbu.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gztbkedyx.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gbyfrttjc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gegjzlgdv.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/guvzpiwfn.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gqhgxadhm.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gaipqvhmy.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gxqzldarh.sHtML


<!-- 参考信息 -->