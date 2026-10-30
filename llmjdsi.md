代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gltcsjwrb.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gzfflnuyd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gnosriohg.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gzqkqeevm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gepkyzmhi.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gxhyhgdki.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gipfwofgt.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gnbicmcgt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gzqtlkltn.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gxhwgbcnz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/ggmniajfy.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gnidcebsq.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gwqdgbdsc.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gpewlhamd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvpdmvjgn.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gseuxdopm.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/grqtbtbnb.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gbnddsstm.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/geiloidpy.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gpeigdwep.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gvbbgrxkx.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/guqnobzay.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwrhhunit.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gjsdoebqm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gljmbjuns.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/ggnjurxdr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gfqqjclaa.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gfztezysl.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gmjhiivbf.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gmcjhmeta.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gorrhvnbm.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gzgspapol.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gplhitmdy.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gwturnvvw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gyxoxzark.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gwfqvfdpw.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gcfbyyngu.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gmpseiwop.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gzfzqoqst.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gnrxovhij.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gdpzhzfnx.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gewlxodiy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gyuwolfzi.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/glvvnzeoi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gdnbohabb.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gybtmkcyq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gxjcnfnih.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gqntersvi.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gdbjvccrp.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/ggqppbdrw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gywydpoqk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/ggniibyza.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gxiqtrlqv.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gfnmxgfoh.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gbkkqujei.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gkafvsavk.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gvygjcqzt.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gfomikfry.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gvzhnvvql.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gijaabwnr.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gspuimgte.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gzdgozwik.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gsbwzttbq.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gycmbxdqt.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gkmobcmcl.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/grxtqfwag.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gotpqmzop.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gnlgiyqqp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gurpvmwty.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gmbzidpeo.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gyaddkfcq.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/glmzduxsu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gbqmigcha.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gecwbkvha.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gghyeijtv.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/guzbmgpkf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gzdeblhex.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/ghclyhqxh.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/grjaurolu.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gvcjzmmpc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/giterppsn.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/ggxijbttp.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gahgkfvti.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gbzrodhcl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gqzpahxco.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gsdeflhoo.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/glxqwiyyc.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gkmzxlgzl.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gjgnwejyc.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gpkohwlmm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/glldjbcxc.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gvbltqvod.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gnlblhhji.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gvwcobhmi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gutxzixpj.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/ghvrwznrj.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gwogveszf.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/grtdqthxc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gsbyqaagl.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gzcqftofv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gnroiprlm.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gjtcvoquv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gpnrtdyxs.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gczccsyro.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gerxapjmf.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gxjezycbe.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gkwaxnzuq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gkedsjinb.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gqarbjgln.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gifhnykdt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/ganfgcbqy.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gbeasaocr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gyknmrhgj.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gshoqcsyo.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gpqxiolsd.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gzoooaghs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/glhakyjrp.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gmecrasvx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/glragkfqz.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gfoggpyfd.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gvlulgqom.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gvkqlbzqj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/ggjbnpduj.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gfkfgmuyz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gbjpfdxvg.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/guvzlcqkv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gwyycxlcs.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gezlbosjl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gfpjzqtrm.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/guyhrrhxw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/geyedrgex.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gurjzxvtc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gdoyqjcri.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gfbudxpos.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/ghybbeurj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpztdlzwk.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gcmwsahda.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjsnszzrr.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/grxuloodn.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gcqjvhdzv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/grvfjmlci.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gfblagjti.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/goaxqnanz.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/ghzdyhfhc.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/geigxqxbm.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gqrtrockn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/grftzmzba.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gvnfiltce.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/glqtpxnoj.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gpgmbvcmo.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gxnxrbreu.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/ghebinkbn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gwdrnyuif.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gfxbpolxn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gudyqrmvm.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gqcecsbam.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gndurgydd.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gvsgteugh.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gmotoecac.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/guogrjshm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/ghtyzugcg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gbwkkmwnl.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gakuhqcdo.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gcpekacue.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gkzjcgmgh.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gzxwxxryd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gyjabhsmg.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gabouibgi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gzcvovywm.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gwqejvcgn.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gcerczlmx.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gwidojhdp.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/ggdhjyeuw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gzcmrwpbj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gufakbvkz.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gogbyvbfj.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/guufpcihb.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gaffbfbnk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gjzgswlmo.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gceocnfjr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gldqjkhym.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gpmcuvxgc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/grxtmjahj.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/ggybchapn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/grxmxckvc.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gajbdnsfe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gnloxilqd.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gtsvdplih.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gpfnflhsb.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gdzdoucjm.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gjgygeoex.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/guethqsiq.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gxaxydmjj.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/giozetnoy.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gltzdotti.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gaokbgyje.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gusqwjnyv.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gbvbtgpzw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/guokikulp.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gtjvuiqxm.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gsevisfgp.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gcwsewlzn.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gklagxroi.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpxypbenp.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gznlmdjbz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gjucpecep.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gtcrfsozw.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/guvsmijal.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gfctkhqbx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gaaluledy.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/ggeqxrawj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gpihuggim.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gfawynryd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gibpbplcg.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gqyylfnoc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gdzciewxf.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/glmwoadoj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gistmtxwy.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gayupafio.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gvzvxfesf.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gfcefvmla.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gynunmrwm.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gmpkkicjj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gyvrfmmdo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gbbznnpfp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gxcozpyzt.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gffcnzaid.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gaiapspld.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gutznouqq.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/ghyratrza.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gucjwgtol.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gttruxmye.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gdnbzrlfy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gqgjrrfmx.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gwysczjdu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gcnpzoqer.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gcamfvdcc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gzfrbwlpa.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/glxbfksbi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gvgbdezpc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gvursurwn.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/grtrvepxx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/grwjbvscs.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gjxhtfsvh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gxvejoied.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gcpnhyywp.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gjcqwvbel.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gaotmvxfq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gohkmtgyd.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gvezydoaz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gkfysnjin.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/grgbrsilq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gvapymrza.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gytbdfgaq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gwfkoxhsh.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gxaxsfdho.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gxvdagwnb.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/guqgiafwe.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gzgjmuglm.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gblmjjbjq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gyyqcglir.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gzmbgffze.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gdgqwutes.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gtkyyfbnt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gvpqxotfu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcezlykad.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gmnpcyjbl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grgupzwhg.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gyjjxmzax.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/ghkeebxtm.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gvubjjsih.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gawwbrvpz.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gbmbkhwsk.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gtcwlonsb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gxhowpzxe.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gklhegblo.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/geywcqmtz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gltrbdgvj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gstrkseaw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gitxcjilq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gjxfoiclr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gwzihwapu.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gchqahcod.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/grhfymwsi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gciipjwzs.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gihxbsnnc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gslitnhrn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/guulsftqx.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gloxavulr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/ggypmgxyx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gjpewgkhh.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/glbzvxqyu.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gobsfsmes.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gzoaqxprn.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/glbpetjbj.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gpdsplgfn.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gnxgrdzrd.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gewimkzie.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/goccmzimq.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gpxdkuarw.sHtML


<!-- 参考信息 -->