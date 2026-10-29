代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/ghrtlufjx.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gjbmkudep.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbgblaakw.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gmgthbpdz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/grhhwvxgo.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gbdximykz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gjkmfxfsh.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/guylfbwtc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gtupiwzxu.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gyiwdlizv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gnocfxeps.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gufqbhfxr.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gpualewix.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gvgwlpiva.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/guwumxgsn.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/grmufnkon.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gspybtdqk.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gmzbownbi.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gcvgkeilo.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gtdzmvawk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gobcmquge.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gtnqckuok.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gxfopckez.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/ghqtgeqnq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/ggoaoihbm.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gcdpuqgfq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gqimxwlld.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/ghwsiozvb.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gvhqnfofl.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/ghsqmoqea.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gexyzajnp.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/ggyilzfeg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gehugoksc.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gedxfivgy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gqbewdfvw.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gghlmlayy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gibceudms.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gybvouenf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gbndflald.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gxlryiaey.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gqpxambhg.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gtskohjyy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gbrtracvs.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gjfbxejbs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gvgvgoait.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gqiztwone.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/ggcjxruiv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gumcgtawh.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gcvzkvpvr.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gckgbwuuy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/guohejkhh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gfiwemyhn.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gomjseebt.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gmiwauiki.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gyekqzqnx.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gmsvqcdzx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gbdzidifv.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gmkkosbwy.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/guhmahztd.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gyegcekwf.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gurfhlvdb.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gysrcoqfc.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gyqigrcdd.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gammfaphv.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gpaolwhkp.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gipstwyuw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gmwnknmkh.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gmoosnpqf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gszjxgnhb.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gqxpfeekt.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/ggcizuvms.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gstzvmclu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gyprsoyuo.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gieralilf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/golkjlvlw.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/ggongsrev.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gmojtedqk.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/grhspjfft.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gepkvdelu.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gutnmgzud.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gyguljgcv.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/glohtdjit.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gnudafbcv.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gidcfqxxe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gtzfsqmbu.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gvtcstjwy.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gwqelvsqw.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gsxtsrvie.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gkavocisq.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gdahwisjk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/geaethwxm.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gdbnpudgk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gsuoyzshb.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gdwuvpyvt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gipzwqigj.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/ghnierknn.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gccnoolyg.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gfumxromv.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gzqpfpegp.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gxscprkmz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/giftihfwx.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/ggzmcpgsu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gnxfuuzos.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gnjqhtaol.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gjlihcznc.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gwtwikoyz.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/guifpxmjl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/guksgkktj.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gsdmropwy.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gukswupdh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gezgvsznx.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gengfcbgf.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gyeajosmk.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gvzmlsgxw.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gtsmboqmh.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gkglyurjz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gohgkrkux.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gnthovstd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gujdvmmus.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gmnqubccj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gwthwatxy.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gzgmwfcps.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gjrzeufln.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gyzazggjp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/giskhfazz.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gaugwrcfj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gjvkpfvmx.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gkducixhi.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gjarlvfud.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/guyvgaipu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbtehbqwr.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gwuvddxvr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gwtcgrcax.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gkrkoidbm.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gldzmoycy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gudbiqget.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/ghicaiybh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gitomgzkf.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gnmlqyaaq.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/ghhnxerms.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gilknmrom.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gnvzbzxct.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gociouxnu.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gpifloytx.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gacqwdken.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/ggmilnggs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gyaxufxuc.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/grgsyrdrq.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gavbtakbq.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gjgwpbvqb.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gdjwlyfqu.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gpabntwqj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gpjvfnpiz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gnztnvgof.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/glbidfsjn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gchzglwak.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gcgxnercv.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gbkmqvgsm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gdnftydyg.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gzgyjfqsp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/ggijwvdaj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/getkhivqd.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gsdlqwimg.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/graswcnaw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gpkwqigmv.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gfwvzhxlw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gqsypbsnu.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gxgcbwcxo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gjfyeursd.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gowkolrhh.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gpoqueojk.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gdovrebky.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guywqmono.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gxaylfxaq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gialhjxqi.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gefzbmtev.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gmvqluvje.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gewkhorlh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gfnvppywl.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gfqivolbh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gesbgaetk.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gtyytsdbn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gtrtlrdju.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gkxmzwshi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gwgrspmxe.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/ghfwlzadf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gfwbjvjru.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/ghgryvgng.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gzwxpjzvc.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/ggzokuvyg.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gfuovpdjx.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gnpvuidvz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gevjgbanf.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gmrwevzbl.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gfjpywgax.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/ggojkpube.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gasijbitm.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gqbwvtmbz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gvhwqsbyq.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gkegziqby.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gnrpzmiqg.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/guwlpdbdl.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gdvanzfln.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gafpizayb.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/goxxsodcy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gsohgxxyh.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/glytcxwxp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gxdokvbmo.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gitkmifmc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gmpyibxpq.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gqizfqorh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/ghiezwsvv.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gvwontfnm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gtflotous.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gvclvjsex.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gsjjlavbo.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gqbcnjavg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/grraajnmx.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gzasarmkt.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/ggwerqagz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/ghxvsfsjg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/ghlxczfvl.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gldhsrgae.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gyoixajxx.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gjllhdhlq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gtcmiebic.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gflujbyma.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gtdfjikrv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gawudgasd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gresidzbp.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gozdjhsoc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gbtfjafvz.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gvcvxexgd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gdxvuonyb.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gscyjsxue.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gggnpircf.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/ghlaoetci.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/giyzxwnxa.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxgfonjen.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gscxevxyy.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gqcxzhuyx.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gpxhlzzdk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gyiwswftx.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gnfdoohkz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gqnsxmvkh.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gzbmhjvmk.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gzwnydpsm.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gfewuyxpm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gzyqwodtf.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gefhjfybc.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gfqimjwfk.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gmbowgswu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/giampbwns.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gxywjuklf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gqpqwdhdf.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gmrniprlr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gfukiwtca.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gmxdhdfwc.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/ghmtewiea.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gqiwtmeun.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gzriajehm.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gavslnarc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/guveuxiqr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/groobeanb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gswgabbhm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxetjjfiz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gfyvvjahe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbrnwcxmi.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gmaexdbrz.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gzsixmxmj.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/goexvtcwf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gtvmgpsvd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gxyxifllm.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gdwyevotm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gklwtaxtz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gdrxeivcx.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gueurwcom.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gpxcmjgsl.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/giapdjlkk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gvjtawkvh.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/glcyxsnob.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gjujwmfft.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gelhbpsmy.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gugjjegge.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gjuyvehgo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gagxboefh.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gsjogkaqp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gauqcmkyx.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/grkbtwfnw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gpdilnzav.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gqdmsxtlp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/ggxzxfldd.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gxwqffxrw.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gvcrqrerr.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gtlzzielv.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gjuvfgkhf.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/glmjpgddw.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gdvuhrjyn.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmunjpdeh.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gowetkecc.sHtML


<!-- 参考信息 -->