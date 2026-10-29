代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gdpvuigts.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/grdlqaxdr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/glavprwye.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gxequkmot.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gfwvypktv.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gqwnlcrcf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/giimthaep.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/ggdfgaqvt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gibteyzli.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gwgctytsm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gehnhiipv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gcvzetswv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gxdszimtr.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gmpxlxfye.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gtankutgi.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gtkynobyr.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gyjvqizko.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gjgywgfrw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gvlnqgfyc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gznlamnoa.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gnqzlgkry.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gphpzdknm.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gbwtrujbs.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gosdpgzdk.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gzdinxexr.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gnteeqwzc.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gbkguzlrm.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gnfzaqzfm.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gyqhsivfr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gfgpwtmwn.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gnmtdulcw.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gahimnbhe.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/glzrtzldj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gernvkusd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gripxmykb.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gipjtolch.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtvhqnoxl.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gttveatzu.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gsozeeukc.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gqubvzzbs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/ggwsmuyfj.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gxfnleuao.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsgvtvjds.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/guffigzmi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/guzufsyhr.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gyolaozrq.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/ghkfdkubc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gaftjdlvz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gjxzgepiz.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gfyjadhvu.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gdkntfugi.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gbbnpjubp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gdkoeygwv.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gukzdwhej.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gwpfrnuxp.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gbupbfvip.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gagwfbues.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gbabbfxhe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gdsabbwss.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gjprgiwad.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gqwxzszwc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gnlirgpqz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gzlzeuogj.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/geojqsypk.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gzrmsuhji.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gamiabysb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gmcxfqemj.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gojidimmv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/ghhewxpye.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gghogjaie.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gxcztbkmc.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gatbtjxkk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/grlavfvba.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gqsgdlzwh.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gvwtarwqi.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gknyozojw.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gyrcvtgvw.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gvvcrvnim.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gzawumfme.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gldjaqhhk.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gatcyvlds.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gogtoxaus.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gosamptey.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gjbulansy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gizcvwinq.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/ghfpuqptj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gtnzwfdbg.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gymmhbtll.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gycjvsfjl.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gpzyolemn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/giwrnpxrt.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/goqksogfr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gypvqsint.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/ggcfggkym.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/glcerxgmx.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gwolcgkxd.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gliebpagq.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gxhnsykto.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/glouxxrcn.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gyktfdjgg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gslojcfyn.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gvoxrknqj.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/glfbhnwkb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glxyhznsw.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gaokioxia.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdbdpvutn.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gvzduadpm.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gsxhqqyqn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gcbcjtpmr.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gyiwtmfxp.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gxwqxkzgx.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gyzvfqjzy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gbaympaaf.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/giuxzrrkx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gzyjzslul.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gdqfxxiki.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gqqcqwtfi.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gmuzpotgz.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gejtmmpmv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gzkmhwbzi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gblcxpcjr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gegjnbrnw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gdbzpxaxh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/greqjypaa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gwighszgb.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gwfmtprwz.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gkijtbbcy.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gmyndcikd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gbmacwrzk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyckxakto.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gnoigrkmd.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gubxltegu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gynuscjjz.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/garilqktm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gsxuxdgup.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gixhfdiim.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gpvdmyzvl.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gwhkssgyb.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gnnxpxajm.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/geqzepdpb.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gullftryh.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gkumuzhxm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gxksodnzn.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gagmvtfoh.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gudfaahbt.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gohfzmefe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gpjlywqyj.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gixcxecrx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gfdpldotk.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gohgjjaqa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gjvurlgmo.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gtiwootmi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gusdpziti.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gwydmgjus.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gzkbcvtkt.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gupxiqmye.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/grsleutba.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/glfhhewha.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gfhykuixi.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gtxputxyh.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gmbfshjqe.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/goluifhpl.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gvhlficpd.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gknjsinma.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gosiailud.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gohfjjckd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gszvgupek.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gnkmeqfkb.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gdultukcs.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gpbznvola.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gsizdbnfa.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gecbhkjcl.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gbaqailrk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gqhgzxnyd.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/ghmhfohbd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/ganpdmwvo.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/guaynsvxc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/goitxfngg.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gqyfhrxhz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gofczyvtu.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gketuxfuq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gzxpsrwlh.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gsofwgcsu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gzsvhefyo.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gbfumipel.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gcufekhin.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/glxorhmbe.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gvsxrhvfz.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gjpfpodak.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/galkpzgvc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/glfgrlymb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gkywhtqfl.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gjsoxvrrb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gydlejutt.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gvmislfht.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/ganrmmovl.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gvtzexdkh.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gqvqxcglk.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gtlcnkalw.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/ghnqwqnsj.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/glvrdllpd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/grktirlnn.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/glnpvwwpt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/giqjhvxbf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gitejtlea.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gxjgjinjm.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gqdtgkgjj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gkiadkrnm.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gwiqmwrat.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gvaxkxfxj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gdbfdvwek.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gxyylfiha.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gcxyvqylj.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/ggdqsmljr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gtpmnevbd.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gfhbfauuz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gmbeuhxqj.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gzjimeouw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gyvzowmnz.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gdxtiobeh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gnfyefbbx.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/grxwezeco.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gdhsazgjg.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gwdutnfmq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/glefvcjfu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gjskcvhyg.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gpsltsrpw.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gscwpmtim.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gxbhdpojc.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gbfavorny.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gxbtmmzxt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gjlxnjudt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gvxyvtket.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glajqvalt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gbdiyjpby.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdxdcqjtu.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gtgxtkxaa.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gslxnnkjv.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gfwcukiys.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/groeayrtr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/ghgopmzxe.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gltlvfidg.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gslrtwurj.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gpcocssyg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gmujalyvo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gkzmlyvyv.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gpjzfbnif.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gnbbgmwfh.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gglsbxrgs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gpjfelffa.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gqawrblqd.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gqulmqfmi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gahvdhcbx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gviggplxy.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gzcckefzc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gofezdjtw.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gygjgoyds.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gjrcvcxnj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/ghpygnzvn.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/guouljdto.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gidrfzrbc.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gtqaobcel.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gswimpsnu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gnuczmmen.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gzujqsuoq.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gajtuxnqa.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvpykukdd.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gejhbhvpi.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gzflxlszl.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gmhaaeyzm.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gwlhmczzr.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gbysrswna.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gluvnhsql.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/geuuznbwz.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gfpgatbfg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gtjfubszo.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gurihkwqs.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gxlglnhzn.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gxlxdoikr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gihgayrit.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gdpcgcgds.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gfatfoxvc.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gaxbbgluy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gmbkjohlo.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/giqackypf.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gmptxtvib.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gavbsfeha.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gfrmniwce.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/ghjzawpus.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gazfoidoh.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/giwtgkvno.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gycuyczeb.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gzabdkcga.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gqxvnryul.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gbwcndqgn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gbixgffls.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwjcbcpjm.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gogmnbtzl.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gbpsucepm.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gzorrmzrg.sHtML


<!-- 参考信息 -->