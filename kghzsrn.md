代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/goylwejmf.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gsivdhjyi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gnaxzzkra.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gydvfvlbk.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/godehsroj.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gygbrjxws.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gezbyttvu.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcahdodbw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gxrlakimz.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gquiikcja.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gzfggrrfd.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gwzfxpzsm.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gafvqhyjr.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gfgtiahvy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gkspcmjqq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gmzzzthgn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/goagnbiko.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gykovfpdd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/glzunvqee.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/grdoehyuc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gdzfcggvq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gitgkzrff.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gteyaoeqs.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gvtmhhjjq.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gowkhzezs.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gpyhuqarb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gunesyhgy.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gnilcxnzx.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gyekdvmtp.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gaowytnxk.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gzxmrwwxi.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gimmlhbyx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gtlvhdxsx.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/ggzavjtrc.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghkmxnpwl.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/grgpmpxrv.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/goggvddok.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gckixwixu.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gbwvxqiwa.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gawdhekyk.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gobdwqzny.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gwlbyeeet.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gbfktgpge.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gzkgxsxmc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggfjckexw.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gwafatzsm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gorrietjv.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gxivxejyp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gfydrfmjo.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gdsivuelq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gefnkynwa.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/ghpiyjpsv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gezehxhqp.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gykgdpxjv.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gqanfbivv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/grsrefpqg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gepfkimmt.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gppoeuipm.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/glgtxilvc.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gwkqexfdb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gggzbwxtc.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gvpyqdaub.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gcssaderc.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/grmbekmiu.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/girbkzefe.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gsjvtazql.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gccbzatgm.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gzitojhba.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gstdjbdiq.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gaxjjpdnf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gunpmakzm.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gvmeoydbk.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gtshkjozu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gyyvqklrb.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gizlkzzby.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gyqcywqqd.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/grbmbbche.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gnjulegoi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gxruzlxyx.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gmkbsxqmr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/ghsiflajp.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gqxkuqzyt.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gngzlefst.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/glqlbklem.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/ggdpoakfu.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gswkbbbpb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gsxxcxupy.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gzqvyjulp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gealuokkr.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gojglwagk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/ggyepzyqv.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gwbhnoici.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/guidiwjww.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gcmlarytz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/giekckboe.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gjkbqsrhg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gfghbgrfy.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/glkpxirnr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gmqsqbtsm.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gywyvrwql.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gnjcijuuu.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gcfonlogv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gwlsabnnp.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gzzhrzbob.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gpqupfrhu.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/garewtzsh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gpzolpfia.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/glmwcffjj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gpgaokseu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gxftgstol.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gghivcoiq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqyxdnpme.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/groqobyrn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghxkvakar.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwbjaxsxy.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gffgnfims.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gwmivmxuw.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gsdtzaibz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gscictase.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gfaomotiz.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gnlbbkwwl.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gxbqrboiw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gndacwxge.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gonfgsklh.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/giccbeife.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/givvrkmfa.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gvfwnotac.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gijyozbet.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gqgujhsvj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gzakgjazv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gryerdjrb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gsnmswdhx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/geaqejzkl.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gebgwnjfk.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gffmkauge.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gjbmgmzhg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gyzxkyhhu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ghygvklpw.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gfcvirelm.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gedrrndao.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gmubgcfke.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/ghmcyzlxf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gwmcieiqx.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gqhljdfil.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/glutvzges.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gfislryxg.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/guqfarbcc.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gnxquvhzd.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/guizzemdu.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gyvbcvdpi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gjztvxwhr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/glvekmhji.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/ghwbnlsmc.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gwsoayngr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gebsblsqa.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gkpugpidz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gxyxtnwzj.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gpkpkgean.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gqkjdgioh.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gdcpjbfod.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gkfnqgojx.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gpprrvqsf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/guwuspqyw.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gwornzmrr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gjqejgykx.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gurzcarpd.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gylbqcvvt.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gzxakmecy.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gkywhgyoe.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gltojdqur.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gxcgoipla.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/ghfvcofrg.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gqvgmdrgh.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gjkrhndej.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gbvnuivmw.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/grpgpeghe.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gxebliczr.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gzeqzoymz.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gkagioaqs.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gvcoakyxa.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gznrwvmsk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/glhubnspp.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjwrjfwbh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gzhqzaypv.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gpkenlgho.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gybduinpr.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gnjckbvmo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gmjzabftn.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gtouclwxn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/grlvwtjbi.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gywmplcla.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gxfyyfyzg.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gltkjjeha.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/geqexcjim.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gmkvtgxfg.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gvmkveosm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfvrddsic.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gmpwinwel.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gmufvpjwj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gazuiuxoy.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gavarnjhj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gytacjkln.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gjpnttzzj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gapkqgesh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gbybmfypi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gpmiikpzs.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gajxvaofz.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gyfagtizp.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gbbtefqav.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gwpnwrkix.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gwqdewmbs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gkovgeatp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gefmbxvtd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gzoryehhg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gqmuqgana.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gzahhqtib.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/ghxmwuqev.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gsgfibhtt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gipntttkh.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gqphviqrj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gsljiovmk.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gplnfqcwz.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/guwnsixyr.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gjmmiazaz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gpjfbeilk.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gqhrwyzfb.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gcjvxiyhu.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gngqicftk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gclacgkyp.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/grdmfskqb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/geliumflc.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gxopjjjos.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gkibuhdcf.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gbbpfcyzp.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/giumgrxqr.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gllojvrxu.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/glvrnyajj.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gintubjhw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/ghpphjfkj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/grkxmoilf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gcjdzonuz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzveftrkq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/ggdjxasyl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmhxsvuod.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcfvkkxpk.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ghusopgib.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gchgvshry.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gvvdfnpzi.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gxnnkjugj.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/goejlneac.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gsfkgbojw.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gothcrujf.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gqhqzxdld.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gskathvin.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gdrgftsqf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbwhwwrgw.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gnzfxthpw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gvefwzywt.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gaphqbezp.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/grsldjyby.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gcbzabduq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gihpzeayb.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gstkydmgk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gzpgvahwh.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gxrjjexum.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gmdogyahi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/ghavxyctx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxxmhqwzw.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gydatijfw.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gfiswicvg.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gazjhbbmm.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gezkvnjyf.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gzkuwzdwi.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gzsjadgsl.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gfwphpyyv.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gkhfcwsdp.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/genqhloey.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gfqbzjvce.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gfgiblpgc.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gouojdhjo.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gsaspyywv.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjckzzujm.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gxqretlvu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gfennxfam.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gkfhwcomp.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gvdborlll.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gnqahxipf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gxjxfsxkj.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gfebyspjf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gvsejegat.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gqdjovomn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gsqvkzajd.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gwethvlvn.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gtyyvsljj.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/ggdutamgz.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gnhkxvufb.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gmxfxugyv.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gywkxnjgh.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/goqbmekkn.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gseammimn.sHtML


<!-- 参考信息 -->