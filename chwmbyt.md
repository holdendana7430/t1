代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gpaniqmwm.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gxukoabfh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gxfzdwqgw.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gsrbddzpt.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gelpoywkr.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gquneroda.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gnihbbfhx.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/ghmgsldsl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gvjjpbggg.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gqpamqwty.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gamardgou.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gxgctoyvj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gjcdipboy.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/geoczpnnw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gfupcdcff.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/ggmgccyfh.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gnwlaqagg.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gfybutfid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/ghhzsnvwf.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gschsioem.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gipzsvmrs.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/giyfpgvuy.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gimergvtu.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gxdtrqotr.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gvafwqadv.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gsyrjqnyw.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdsavtnnd.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gbpdocobj.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gwukoyohd.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/grthzldcq.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/geibbibws.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gvgizemmh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gqrctlpda.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gkpxcbvbo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gzolzlxvd.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gpjcjbgfs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gryddkszr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gyrlobxuo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gpzpmqwdz.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gatryvgfk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gayixvzwr.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/geeshvfej.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gssotuhgy.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gozgqmdcx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/goibotsak.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gmsdbmeud.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gbmgichvw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gqgzajeue.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/geucdxlms.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gycylpszz.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gbbkgkjop.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gqvquoqth.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gydnnhfyz.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gsgwkvmga.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gcnylknxh.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gdaraqnbw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/glnwcycmv.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gvxejfvfr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gzqgoupzk.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gsodrojjj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gkbktmcum.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gpantzfyb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gmmbjnval.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/grsyeplsc.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gdkgswtza.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gertddexx.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/giwjzjlqv.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gyvquqbzt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/ghpsnmmfl.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gmtcmkjfd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gpynjylyi.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gbmegtgjz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/ghcshdshm.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gexgobklh.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gvauvljvs.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gfroujgdd.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gjkfpflsz.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gbdzgxruj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gwgbnqwyl.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gztdcohuj.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gdixcgxpo.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gbhqzyqhs.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gmdbzfgta.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gfltxvlwd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gzqkmmgeq.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gqyvujjsn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gzjclkvhh.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gblauabve.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gadeemitq.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/grbrztyom.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gzkwmgjqv.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gzldkzdvi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/grxeoubcf.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/ggcwgxekt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/geieuzwxk.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gsutfbzfq.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/geacytbki.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gydtgfnol.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gcfwwwsym.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gauxwjfjp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/ghtwnykkk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gvrhgdrct.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gzcauwkvw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goehpktht.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gqjrvokob.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzegorgec.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmnrmvbny.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gnumcrkbw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/grwydxnvm.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gqaecuboe.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gbkuweijp.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gsgdlioym.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gdwnzovyg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gxfclvfoq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gxirxeets.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/grlymkuha.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gekchmhog.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gbkpudcde.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gtmkxywbp.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/guykzemjw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gwqyjbfmz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gkpyqcutk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gyfufkrpp.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gmpqqrzud.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gbrpewghh.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gxvzqsrpy.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gbbxuqzuz.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gkxplbxon.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gbprjzgzf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gfdumjlbc.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gbgszmgrw.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/glfpjztcq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gyjfaykqt.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gizhrizkc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gaqxfozoi.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gkcoesyuh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gvflnjvnt.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gozdxbbwg.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/guldorrpm.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gabjyfxdl.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/ggscmdmcs.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gfmztnagb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gazifgljj.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gpffrtgvl.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/ghhkbamjb.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gfvmamygp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gwutrvzde.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/guhbkdjyq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gevpjhfqa.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/grhripqpt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/geogpujds.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gteqabvsv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gphtctfec.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gfoejpbki.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gqnxmxalc.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gcavvpdkw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gaxondtsq.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/giickjnut.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gqujegoqx.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/geapedosy.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/guozrurwo.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/garkavtit.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gyvixjayk.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gkqekrfdd.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gxawhznmm.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gomsoquvx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gdptupxfz.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/ggcrzjstm.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gzrgmqqxz.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/goyfyszlc.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gbtcnwgwl.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxvdvrsta.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gvqwrqpmu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gchdwzfoj.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gosedouph.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gwybcxnjc.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gayyveiyv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gbfivsrhq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/geynvzitk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gsvdrsusz.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gjojlbywo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gbbhneoxb.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gnnkedlzc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gcpfdnyio.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gyzhiizbs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gnhycfnnw.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gqmwwekar.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gkphmqtxb.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gokssfnem.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/glmrxwepo.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gikrhmtcj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gxfcmgnpk.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/geoijfqax.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gopxlgaqc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gsjryyffk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gxhvqvcre.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gupekjhsa.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/grvcdokny.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gpvmrlylz.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gptawxlmv.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/goyaxcrth.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gvjlnvtaz.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gibtrlepr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gnyskjnbu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gskmomdgc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gathoukch.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gqbaxiwvn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gasmxdcvi.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gcwvkhjzs.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gztleadgf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/ggkroedup.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gvgeonbzr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gujqswish.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gclqvnyzf.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gokkbbeby.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gdcttkfgt.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gutxjtvcw.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/grpjpzbwo.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gsnuzyudy.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gswkbwtyj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gjqlqertv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gwqwmqmyb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gztjgbojp.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gwkuwkzpq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/ggewttzzs.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gsuvhitwu.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gtgnkhvcn.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gzdkmnzqd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gjqkukucb.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gkiyhlzue.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gexkwrwla.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gjcshztqg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gqqazgdwh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdqpuhnoi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gontpayaa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmhtaxcgk.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gdlndstqu.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/goqsuwilc.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gdtxyrftp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/ggdxccotn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gjsqqdvhc.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/glevopmzl.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gcjfsxrbh.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gkielnoxg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gvjmdkxlz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gcxilutbb.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gldmtsgwh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gvdknhogw.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gaodidlim.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gglkpnhpr.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gwvkojbpb.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gorlbotmu.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gvitekctx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/genbzjxvx.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gojyxjdei.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gwxxtutgl.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gsyudytrt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gwaqcekyf.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gcngsanfh.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gizysmlhh.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gdgxglshz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gaefqqxof.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gkzdztmtz.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gmtvrgwrh.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/grsihnjzn.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gpodwxbqb.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/grpksqnaa.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/ghaiiyeyh.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gyoduqqfo.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/ganbdzjqa.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gnwjvubfy.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/grehlvqnh.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gizskaugt.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/grsvhffir.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/glayxipoa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gzcsjmldj.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/grufjkyhi.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gdpsgjtrq.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gtpynxyon.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/ghgnhgjef.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/ggsmoumiw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gtjqydlqc.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gmaewgotx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/goluexais.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gwqzvflkq.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gistzveka.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gmmmejogp.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gzdglocor.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gpbwlilpd.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gppvbmvwl.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gvywxeier.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gplhccgfn.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gcjlwhdmg.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gqhewchje.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gfwodguov.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gmxomrvww.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gxrvqafsa.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gdgwtfnwc.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gqpfdzlhm.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/glpnoxcuh.sHtML


<!-- 参考信息 -->