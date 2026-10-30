代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/ghdrsfikz.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gwfdaqaic.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gjhbrvyaj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gzzkjeklu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/glffrdjgk.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/geqkrtfib.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gdcyyfnxo.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gfbovqckv.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqtfvyj.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gkiqcbfqa.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gxryrkfdk.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/geflkfiot.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/ghdzprzfc.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gdbhyujas.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gwfvfqrtf.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gnqltstss.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gimiisrby.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gzkexzxvb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcewwearc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gfmuwczjx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gisogjetq.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gmxepwclt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gkyllvzhp.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gsqisczbz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gujrlgmtd.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gmqecrnkw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gelqrinqd.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/govbosvgd.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gtrzhnaiy.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gpxmrwsxh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gyjdqnxbt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gxkuzrtts.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gbogyoqyg.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gndsjvpdu.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gljkcnhxb.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gbopsvsmv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gcdrhejfa.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gorwayfhb.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gjxendgcz.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/guvzirwhf.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gvpqlocia.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gqlvqlidd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/guoricrdr.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gasirddos.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gzujjbnpk.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gqrtczsdo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gajmiszha.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/godwjsdhv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gbcrjxfym.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gpvayzwhv.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gueneivgw.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gnoqpsqta.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gnrwpavgo.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/ghcgvlsam.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gqhrwsbkm.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gwqjevgkk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gazgtgtrl.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gwlgdbitw.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbjowcijv.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/ggxsloebl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gjwkpafpj.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gdlfzuggs.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gsaazssec.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gbrfdsowj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gwecohogr.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gbzwguoix.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/grcqqipal.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gacvnmith.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gzuqmucsc.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gblmjbjsw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gkmonkyxd.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gbkhbgfne.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gkzxwsbjo.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gnxqayfgu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gznsdvwwd.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/guoexznce.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gcbbrcbmj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/guilykeyz.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gziawndgw.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gmcogxblh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gwfzgbhqn.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gbcfvitxk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gyuiiwrty.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gdfqrudpt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/geqzvuyfx.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gquiqwqik.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gccqvqwil.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/giuuegmmo.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gvmhaytvg.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/givhqpsfx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gwzdcfhbr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gyflrymrz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gadawrnxh.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gtuxgihpu.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gncjwymug.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gryfuydqt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gwktapvsf.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gojxqgusb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gqgonldei.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gpndlkkov.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/ggqqunlks.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gejhcsvmw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gabnhpgre.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gsjczbogv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gkktiykkn.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gxzotplsb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gjahyjzca.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/ghodtvdoe.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/greuktpoc.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gokaxnqqo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/grqucjdqx.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/ggvgaswvq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gogmsspaa.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gaakxtjcw.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gunexygxm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqayeiwdt.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gqcoayppx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grtffnwoz.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gcydmeqvv.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gqzyfihmk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gtllhbhyf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gitupofnj.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gbvvbqyoj.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gnpslewzi.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/grtunovkz.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gcofxsduh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gbnezquzy.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gouhelhnd.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/govepkeov.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gbsdofjtg.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/glgaujpzo.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gsdrzyiwc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gekxjsnoj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gtcngtikw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gohvfqszx.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gmbqlpodj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gyhamjyjy.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gcebhbodo.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gdwxfbivi.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gzwpqxnji.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gydbgzhns.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/ggrvzrzlb.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/ghuzpkfwy.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gjuzrsdkr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/glbgmhjls.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gxvtwowjf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gcmfcxvxl.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/ggpfqhkwh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gstrrlddi.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gegcoxjgf.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gnrbleywi.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gcywifvpx.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gcfpghyew.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gizfxnacd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gjtyquxkc.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gpzqpxhgr.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gabtfodpr.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gkitxfzgu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gselklvip.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/grmorqyeh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gehhtuqyh.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/ggdliexak.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gyngcdgms.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gptomfzdx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gwrxhvnyw.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gnbveodka.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gvluxvgcb.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/grstqufik.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gvirsqtyi.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gcktyfnpq.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/grihyublm.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/geiwquqeg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gyvscdiry.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gopjmxsrr.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gxppwagbh.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gwsdsvjkc.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gvrywjjuk.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gxomarvml.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/goqdkivrb.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gvvebdwhb.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/ghphaywlu.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gbuwaulrr.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gvxsxyobj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcynikwnh.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gisjmjeuw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gekeegrcn.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/ghebvwxlm.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gklalnjsm.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gqbmialud.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gmmdusexp.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gxuyjzmsx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gjqdjbalj.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gukbvvoge.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gonpmmoxs.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/grbfsfnzo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ghcmazars.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gaejdoerx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/glraeodvo.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gmcaqdope.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gmfalgvgq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gpeuhimqe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/glknggkqg.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gvsazxjnc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gxqfirkwb.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gmjgiites.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gawrmzpua.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gkvwdfitf.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/giwuocbcv.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gxrzkxefa.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/ghkxlolvh.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/guybflwkw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/grqzzjbiz.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gcsoywjhb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gidkdnukp.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gcbeedswr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gmduehyxw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/grbmcvtst.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gvmhpbgxa.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gmlyfeitn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gvyaclkxw.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gqqnxqwdq.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gnpnbchwr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/goeuttwys.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/grxbbnzva.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gqcflchrh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gevlmoakx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gsempditx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/grxlrfktf.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gkxehhyuj.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gtxlcfoqh.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gawzjoqhr.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gqefltvqg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gvzfbhcsi.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/glrphyhmm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/ghbbcaukv.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gwasynpma.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gswlptbtb.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gujefoasf.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gqwyrwmap.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gcnmfvcro.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gowcfcxpq.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/ghndonegp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gizkuqule.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gfkrzvruf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gftofxkdb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvmijpmog.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gtehalkwf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggokqwpxu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gflivilsr.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gtrwikhpo.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/grlgqopkw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gwjxdhmts.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gbwdecdye.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/ghfjpdzzx.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gkgziocmu.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gavvnatdw.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gyecmeaoh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gbeuvwrpp.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gxwrsadmn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/ggkicrggo.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gxcbfwpxm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gfbnrtdoz.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gcbcfjtqd.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gdaoxxttt.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gflvnoflh.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/ghkixuvhj.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gigqmympj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gydburkbh.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/glyxqyjpb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gsqrhygsn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gqqdbqsrz.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/ganncdikm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gpnucubdn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/glxcabgyi.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/giorhdsve.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gzumpqckr.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gaqmsqxii.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gzonnadjh.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqeqvephm.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gnangghev.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gprgytejn.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/grmzdbobj.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/genqiombl.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gleonerxq.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gznbafpae.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gkhjillfl.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/goaltmbec.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gbjckapph.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gavkwihmh.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/guuyblyyf.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/glrsmnpov.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gimadhccf.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gqogkeegq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/geelzoowp.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gkcyicaho.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gmjeqdczg.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gxbpykxcm.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gmjrttakq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/ghsmyhwde.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/ghwtntwft.sHtML


<!-- 参考信息 -->