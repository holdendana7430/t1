代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/glymcylan.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/glnkogyak.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ggedzittl.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gsshhwpnj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gedjelfln.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/glhjofkzh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gcbfsznlk.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gtmfjdqlm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gvuodyoyc.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/goruaejwz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gvwatgazu.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvnowwnuy.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gzlflezdg.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gvbqwpmwh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gqyfnnpcw.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gnvagvvia.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gcswjwshe.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gmvrqfnwp.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkyxozfgc.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/grnirxohz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gpjylqdul.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gmsmauzax.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gqudmycml.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gsnowfzak.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gtyfjprma.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gkimnfiop.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gaoozgnda.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/guqxjzxcl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/ganztqkxd.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gezhljowu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gdfzczbnp.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gewowkftq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/ggztgudmg.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gmagtceoo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/guowrtsld.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/ghfeitaiq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/glpsmmoep.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gvfargimm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gnoaebese.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gsuilpawx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gkejbplah.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gsjlvppwc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gfgiwmbxk.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/grpnmaghq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gdphrxeqq.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gaoqwpdtd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gjbjebjrw.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gbqaqckde.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gqfarumqj.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gnlaabkgz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gqpoqfbsr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gxoixnxkq.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gkbjqwzhc.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gkfkoiyzr.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gbiyxtdnn.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/golzfyety.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/ghdahbuuu.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/glivzgujl.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gdjczogdq.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/ghtrkupal.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gjyzmqfjs.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gavsumzvq.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/grwwrykdm.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gkmzbbaqv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gxecasjqs.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gzkqiflct.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gqaqubxgx.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gbckoyljn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvqkxdgkw.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/ghaqmqzvn.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gsupkmtle.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gmnplvrah.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gtirjnpxr.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gnixcyjxm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxthvzktl.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gakqaaqxu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gackqyqav.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gyiwbcoaw.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvwseomtg.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gsicyzood.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gpqvvwuoz.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gjpjxzixr.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gjtyrknkh.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/ggxozlrfv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/guxvkmvgz.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/ggenqyssy.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gqrjkniup.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gladfrram.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gmrzujqqf.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gueabyfri.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/ggvltrhvt.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gkprkbtmf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gpvvigbcr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gqqpbzvrs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gteposksp.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gubhuosmw.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gonwefyms.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gwlbsotdf.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/grfsbguqi.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/ggmmfkbxt.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gxmvavufj.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gjphopntj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gqqlxnvze.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/guqnytisp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/glakjeoni.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gfqydrjvr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gwijpskxe.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gmthltpvc.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gnoafozaw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gcpwyfwuf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gcnmvzfgt.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gznrwnjro.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gdnoowiyz.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/ghazfwhpu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/guikfstqk.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gcipktrsp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gdwzjihmf.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gxsebitfv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gmbqcvjnc.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gycaqkrmx.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gwftzsfjf.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gmzvptelt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gacuuiwag.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gnashsjgh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gbhrwpocd.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gqhnveept.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ghuavuzih.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gtfktslkn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gpdhofrme.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gnoxcglst.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gywduepig.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gwcryobvn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/galpdcncx.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gyzzacqpk.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gpqzgtrlr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gppwwfcdh.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gttnsgbaf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqwtjangg.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkvzuqsgw.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gixmgcgzr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gsbifeqkn.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gaacmgvvq.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gtjdiyxuj.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gpjexgxep.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gqnsfwspf.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gvnvjdldm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gcguxlgxx.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gleelbygz.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gwxgrtuae.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gxhbytesl.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gvjeuwmug.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gocvzxsgm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gubrmjboz.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gaihnhgvk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gkktqluek.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gclcnmyaj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gthclxklz.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gayhgwizh.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gzqrrbasf.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gztprucvw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gzjtmthyd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gczvsdhfs.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gpfzxiqrm.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gbdqgkgmc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gdilisabi.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/ggwzyqohk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gypfocaqs.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gqsoxsduj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gixayrmja.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gtidcasfl.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gzmgtivxp.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gqajzjyip.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gzpggoiwq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gjctkordq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gbgpcktgf.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gdtejhfhg.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gbzpqdwau.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gqztdxyxg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbhzlqzw.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gwyigipji.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gniepiceu.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gikxxjiet.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gelrvgqtj.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gkiobvafl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gevttmmlt.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gsqmuaube.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gcwwdvxvh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gdphpgayl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gvjphmtlp.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/geykeffzu.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/grhnxcfet.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/ghyhcycwt.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gwulwpwki.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gxslsowks.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gygdsyvfz.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gwowgepbi.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gupaumuda.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gbkghkgut.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gvzhfvjqo.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gxxsceuus.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gwjkolamm.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gipzjsvie.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gukkqewth.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gbyumzkow.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gnexpaatg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gicukqwkd.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gardxmwaf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/geidexise.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gyevebvzp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gcpaakgoc.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gbmhlkxyw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gasvnfgik.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gdfcktphv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gjmpbxrcn.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gzmrsfmlp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gfnwgfowm.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gjlyakvdd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/ggorbmfbt.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/geccksagh.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gqiojxlqw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gpiejddbt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/ggffkzevg.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gdouupgng.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gamkklogh.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gcqauefet.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gfbsuvscg.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/grbqokwwi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gqvtkqlcu.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gnnseduxd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gratxmvmo.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gusyigokb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gebrwshhi.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gcwthymdv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gzbclvetq.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gsrgsmsnb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gokzpzryi.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gwlfjikdi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gvzoqqbwz.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gmejzboqc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/ghrsmnucr.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gphgafejk.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gvjqrlrxw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gaizbxwjv.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/grznjphog.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjzaufxdl.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gaweghpsl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gqhbsrcpv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/ggtghhdbh.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gncojirwq.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gegiqwjlk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gipmecqhk.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gmubmyrsy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/ghamtdajo.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/ghpfzkjve.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/guydayypf.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gnlieengd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gvpgxrvec.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gecmthbqa.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/ggujvpmcw.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gktpngxxv.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gtvigbdlu.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/geiopuvpa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gehobelax.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gxwbecdpw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gxftkzula.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqsllvznv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gtanvnhux.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdsmmziyq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gmdbbkclv.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gtxajgaqd.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/grtvlpagu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gyksrqjzg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gdshqzlyb.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gxctyvqqi.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gxsxbzthe.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gotwmwegq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gqoeyxvql.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gilblqqgo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gakwaqjuf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gsqahlazm.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gfgmbqtgr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gsjthjakh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gpeaohlpp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gcedftimy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpseiqmum.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gnouazbks.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gyzipaxqu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/grcexjoaf.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/giauhvlhg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gnexxgfgh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/guxccjmor.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gisrgfgqi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gxcnqkgmu.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gkqjodyoz.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gdsmscqwl.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gpscgdpax.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gycxushgc.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gskcaojkh.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/glbkmedcl.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gtwyebaty.sHtML


<!-- 参考信息 -->