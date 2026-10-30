代发 wailian999

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gzvvvgahn.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gabkayhgz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gtbfjmdrf.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gxhkrbomy.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gjsebwwqk.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gxjwdgujr.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gsanxmpsl.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gughfqfgq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/giujgbgtv.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gbfzaiwtp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/glglppbjr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gbqxhkpky.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/glbylvlfz.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gnyzxbrik.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gwaaqpigr.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gmnkxprgx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gkmalkmlp.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gaytgmnio.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gpgaxnwty.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gkhiuzxyh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/ghfynchvv.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gcphghdar.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gkznhcevq.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gqzsmdyrk.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/glbvpdikb.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gjkzezhxx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/geutkvqlu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gvjjsoehy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gudrffbjf.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gztvqvvfl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gwlmmbuia.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gbpymvimg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gcefzqssw.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gixeloqlu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gfrduofgn.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gnxskjnfk.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gxcsymrnb.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gfrxcvupo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gvibnxynw.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gkvidwdfm.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gvgjdiujl.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gforzisfx.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gxedddnqa.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gdnjdefvd.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gllfshvhm.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gqkozpyza.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvekayjgo.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gebnsiyur.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/glcxkfhqk.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gfigkddwt.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gkjmzvvhd.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gwogwvgqw.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gdpjgiocy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gizrbnuyd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gvhdpivrj.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gctdivyig.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gcnupwkyc.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gfestkvpr.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gibhbvoje.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gdblbcmlu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/ggugbwrsg.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gfoacqnne.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gvwbwzacw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gtlxmuxku.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gnpjqiepv.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gkjvgskyu.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghjopnvgj.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gmiwqpohf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gwxzsbtan.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gvyebddpo.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gvzlcydbu.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gkmotngvj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/ghzhqapss.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gazlonrbc.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gbluatwmg.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gjhbpmnre.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gbblxsyxy.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gxxxwgoos.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gdckzntqs.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gtyaxkwby.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gzpkfjedn.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gtifytydu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/grhhgsrxr.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gzavjjyts.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gxweafydf.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/ghqpoyeeh.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/guufkidlh.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gvlkyamhd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gjhmyobdu.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gffkpyjyj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gtfnzulup.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gifjlxino.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gngpnlkkv.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gbzincles.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gkotztlga.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gahgfxknq.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gulwdjvgz.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gobymzrlf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gajpwbyfv.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gdprakmwk.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gjuyudihu.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gslwxwnix.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/goorielms.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gzqjjldca.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gwbcgjepv.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gconsquma.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gmmobzcor.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gmnwilhtp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gbtjzdzhl.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/ggfqfjvex.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/ghpsrnymu.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gzuuspehl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/ghcnryrfr.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gtdsqxohd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjuogwjck.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gkwzfqhzj.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gcbkcroum.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gkduajiwi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gsjzvymtt.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gwnxgvovk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gfudnqxgk.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gylvhglel.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gifwxtlcn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzxytjxig.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/guvbnlmnu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvmccypnl.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gblvcllnt.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gbvpfwhrv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/ggohpzrco.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gphymsrff.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gwkjnqyih.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gyydtayrg.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/glforezvy.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gsavfkdnt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gnjjyxmsj.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gcbivmcrp.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gvflijzil.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gbolsphlq.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gvpaofaer.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/grupfjzhh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gvjuqprym.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gwjhzmyyx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gqirtlrdh.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/grhkffbxu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/genglkuje.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gtrhgniyb.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/glvogiwhf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gdavnegym.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gewblkvco.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gddlsonyq.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gteapvvfv.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gfdbmzxta.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gtodwmebz.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gxewcghqs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/goyokdogk.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gsfyxzzfj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gluqaerun.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/ggtusyucw.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gcqmwgkch.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gvvarnjjf.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gcvipilsx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gstbyjqxa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gbciatgtn.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gtihcdoqs.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gpndwppel.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gtluywzri.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gbqwfdskf.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/glhhzztoz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gpnlqprvi.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gpmtktsun.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gbuyxuypo.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gcnxseycx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gdloaaazr.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gdgetshnj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/grhjyzlvc.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gmmcaphkl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gafhuomhd.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/ggdeokbbo.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gqpvvwncl.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gqlaygmgm.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gknpteuwx.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gpieiktev.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/ghakmbwwm.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gtckshfpk.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gqbvwikhs.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gyeugbavc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gqwrjrtdh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gwhgtipxe.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gbcgwhzua.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gkopoqlvb.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/grrutilvf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtblibxlg.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gwwqsbuxw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gxcqrklbv.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gfjsqvqcl.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gyzdstnoj.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gnmcocyft.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbhcrugcw.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gilzaifob.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gfkpdjwlv.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gpyhylzfa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gvggeeyzv.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gfvuzlqwk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gfnxckurl.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gcirnmadj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gsajwmzof.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gkdprbjqz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gmlwmzort.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gcshnaqvr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gcvowrvbs.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gjiffwyli.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gflihbiij.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gserggevd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gyzunwzpg.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/geeapjxqx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gfpelpfqh.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gogqbdpij.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzssahcf.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gimfznavk.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gehjgivtm.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gxcheuwww.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gxvdlqdqo.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gvobqgifn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gbqjbmeaf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gosuxyiaf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gmchlietr.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gfcvqmyrw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gkkbrwvua.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/grevypepo.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gsotrtgfo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gjjpbrvwh.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gwrmkpfjw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/glbbhkccx.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/ggrhmgihj.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gugxmuwgk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gzsbwrqcl.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gcjafjoak.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gzlvgulyz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gwbpjlzeq.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gndecfwbb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gfpqexhxd.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/guusulijd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gzrmkulhn.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gxtoeoumu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gprcffiju.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gsgzshszl.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gekbwzlde.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/ggdipxlvb.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gpdzbvmvw.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gpqgduyxr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gzydwpucb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gzhdtbccx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gmiyszpup.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glrcvhtxp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gwjjyoeja.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwkulzpbo.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjgajdhbe.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gfbhpwiyv.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gdiiiijal.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gljmvqzht.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gjtumhkoh.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gvkgmlnnp.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gbuabdxva.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gzbyqixtw.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/griyexooi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gfclqlrzb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gwouiqybw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gemdbjtjb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gkzqrxige.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gqfhkczby.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/geiuwjfbg.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gecpumiwy.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gqusxistr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gznpfyywm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gwrowokvk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gmnwhmpmg.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/givrbmuwd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gnmlznwwl.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/grilzfica.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/glmozrsvw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/grtlfsrzl.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gezwrjvtw.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gdcolvqjz.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/glgtvonej.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/ginhxhclz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gjsyuujsz.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gvtfejewo.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gsddkhynr.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/guadoqene.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gnnlnoguw.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gbwlxvhhb.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gpwverikk.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gjamdrahx.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gjuraajnz.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gqxafqmzl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gnsghflwl.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gyqqslxhr.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gnqdmyzlu.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gffawibdm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpqsbrldx.sHtML


<!-- 参考信息 -->