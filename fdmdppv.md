代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gkhynnprm.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gndgnrwfk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gdcbscckg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gmmebrruo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gunmgiaie.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gpczdauek.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gwvspprfp.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/guvnfihqv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gorokdbvo.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gujzhyepg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/ggjrciwhq.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gwxsmbkmz.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gmnvtdebv.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/ggbudgduq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/ggjiouluc.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/griwrqprh.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gbokrvurp.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gevyphvlj.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/grgwzzcsy.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/ghbwpponw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gnqsjdcrn.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gciobajuc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gdtttbqlv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gditulvom.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/guadxqqca.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwwsqmwon.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/grccwvesp.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gtaztdfew.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gunavvznn.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/glevlbvzh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gzrhbipfe.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gjcunqxbt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/ggnduvtuw.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gnrurouny.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gzgyuzusr.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gemecovzi.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gxrxjcqks.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gimsugxmt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gkrrzfscc.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gqyibvyxp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gybmqafir.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gidzxafha.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gvvdqgbky.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gfjtgnlck.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/grtsenvbt.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gwiviyrwe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/ggrzqjfrw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gbzngsvwu.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gofeidghy.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gjmmysywk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gazrnhlcz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gxfjrglut.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/grchihwwg.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gjmblfrqn.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/ghphuiauq.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gororgnfo.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gpzrqapxf.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gxuaozmsk.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gihzjcgyg.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gsaukhmfy.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gszylcvnb.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/ghdqtxved.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gwfgmukfy.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/ggdirhlsp.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/ganifhsgq.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/ggiszvmzd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gmnrastsd.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gxbnzimon.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/glozeyrpi.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gbmpxbrzg.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/glallumrd.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gfcrklvcc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gsoaxrkql.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/geaajbodp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gpjkxdgkx.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gohwitaac.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gvadascys.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/guiqgbkbh.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/guvgvqnkd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/grwozinqy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gksmmbudi.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gedxbbwvj.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gkipjymmq.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gggkxvkxx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gaszacwfu.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/glpvyuaqo.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gszmyzwnl.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/girxhaced.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gkptiswbd.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gfvqvudff.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gsqnuchtb.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gkvzmsxjx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/glcdlmtnw.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gntfhpmqk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/grphxmejp.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gwydaolxn.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gmcbzejjr.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gygmxdvbf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/guadivdwj.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gztpwnoqr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gvohkfpnd.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gxoatmsdu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gtimljvoz.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gwuzqohmp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gqjucngtk.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gwqfodcfm.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/ggenjhvue.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gvphosyyo.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gsbnehzob.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gkvcrmoec.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjutcfpsa.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gquyzkxxj.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gxbtesxxb.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gguilyjkf.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gvxybmozt.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gohylykua.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gategfbfu.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gvbhakfjr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/ghgovqthd.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gldorpymr.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gptavdlgv.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gmonauwin.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gwelosdou.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gokbqgwyf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/grnnpgjus.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gzupaecep.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gwbcclzrf.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gotbcyteo.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gzmovjhzc.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gngchxyex.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gpmspqmbv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gchuwdrzh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gqdpqygly.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gtodsijqw.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gwfdrghcv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqherotjg.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gzorvkfom.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnpjceojs.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gsadhbafl.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gapjoacvd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gkfffgnkp.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gyhnkyufk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gpdtsrwww.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gnjmzkgjb.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/geydqopyn.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/ggvposisz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gmxhtpyrj.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gtqpvkgaz.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gfmfszwvf.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gcvjknash.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/glawqluwb.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/glfwolexl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gcysjubwn.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gezrhusow.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gcgduatql.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gxppzdahe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gvknfjhav.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gahhanbpd.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gyltgpepa.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gwcdrhbqw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/ghutznzxs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gcakfyjeh.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gkxhkufeq.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gznjcfjpp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gegdajyei.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/ghaalrlzm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gfinkdapc.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjkubkheg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gihhcaacm.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gfmpzyxlm.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gbvsmcgfc.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gpuxqlczz.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gucsygzum.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gujkjhnfl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gvprzxwiw.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/goazjkzmj.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/goshdwgin.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gjpcnhyip.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/giisauuqm.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gwolhuufd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/ghueftcms.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gpvzzyzdb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gwbbmyuaz.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gnevesmuz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gvihtpwvx.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gjnmrapbm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/guthrroce.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gyziozjwh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/ghzfsgemo.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gkdotnuwc.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gajduilxh.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/geyhqgiik.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gklqbumjw.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gmgkxcize.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gahbhpyir.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/guslakhec.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gxwjywdde.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gdhaxeloz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gsbezvkgj.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gkhcklhby.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/giytnropq.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/ggvraftzt.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gpisikovm.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkfzaevwv.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gxccgveze.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gnutfxhuy.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gikzephvx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gyklrwoui.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gbyaehvaz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gowycmijh.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gwethsonv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gqdsiqjol.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gruaritvx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/ghtmhqpqq.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gxvoubdhz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/geapxedyf.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gummonfsr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gcupspmoa.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gtaimugst.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gsgcildva.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gxafbhsch.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gyykkckag.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gwnfdnrea.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gaoyvpzqd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gachkqhha.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/grpikeecw.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gsjimkexo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gzzxrybsu.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gbntiqivy.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gxfdphpil.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gylkquxym.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/ghqljmxuz.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gpjnsxndq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gqtwvfjsu.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gxebhzmgh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gvxumaoon.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzefchkgd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gqkjbxylk.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ggjvfvodw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gihmdhmej.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gonduprmm.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gqdixbgpq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gjwqrigyc.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gejefxxpi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gfxqejepv.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gaclialbp.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gsyhuwtci.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/godmrslwg.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gvhpxhllm.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gvaaibibf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gadahotxr.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gylyjsmsg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gcgvoqdyu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gsiolercl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gtkmxpluy.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gymciryhp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gosewqhaw.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gkeeehprf.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gkxnjfjve.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gfogvgrbn.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gmskhsptn.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gkyclllcz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gfyvprdlh.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/grppgdeix.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gsoyupuuo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gidslbdpu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/grsvwcbya.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxohzinxs.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gynpnlmnn.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gfvskkfwv.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gvthmvxrn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gmbqzeoju.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gkeqizrky.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gefrjtdru.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gzwlrmlsy.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gcawpcldl.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gdejgscuu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gdugooyco.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gfgutghxt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gtbwegkqu.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gqvytmxsz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gpvbpbioh.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/ghvpwbipx.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gareiqwsf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/ghqhkjvyu.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gzgxzrlhb.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/giseuqalg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrwselc.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gfcuhznfc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gxblwjmmw.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gulrumgch.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gfbxwhish.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/ghejqtlfn.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gfoyepwkn.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gfalmfxew.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gogcbtkzp.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gjelodldg.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gzjorbmgm.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/guxlltyfu.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/glpsovlyl.sHtML


<!-- 参考信息 -->