代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqxxeody.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/ghdbbrsrk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbriyqog.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gttfjqkqy.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gotyiaxgp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsyrtdhh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkmspwvv.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gixuangmq.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfxlithq.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaacuoyu.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyctyxjqk.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnixwzdxh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztqeychd.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gyellgpks.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdaofwkv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoncgwnl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/girhcohii.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggbbksejj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gtmhktnoh.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gikqhbpir.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/grybmovoy.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gqloqqdry.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gckawqoql.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gobdqpikl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzsiyvvg.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvvdwdar.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gapcyhxva.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwybsbnza.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkkeaizsh.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gzekbuuvf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrceheja.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gamcvhwbj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwtjmnqa.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gcauxnsat.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gujsfszch.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gzspsfwmi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gbwkqhkcm.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyhtrnif.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gvubgcsiz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjglrnzix.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwkhbyujq.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gbctkpfhq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gpkoccawv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gaafrzvlp.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gobwdklfy.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/goozjxowe.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gmuvwrjbj.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylcgztyx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gyotbzahw.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gnlqqqahq.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gunzjgtah.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gveqgwtiu.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxamhiku.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gaecmieoc.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/geuvssorc.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzkyudwn.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrnemsnq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhwwvmwt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxwqwgre.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gttagipky.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsgasmhis.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssvntqqg.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnacejfpn.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gwppepkow.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gxujniqkx.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gpjoqjmau.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glqpexckl.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/glnfazfiv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gnflzgytc.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gneksrequ.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbjzdaslf.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoeywnfk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltdvuyvq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblwgrhxc.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyltpisve.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gysdjpwoh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdynwkaro.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/guceczjge.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcggqhayq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtyarzek.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gsranibcx.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gywfmvdsc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gjwfsxnoa.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gqffeivaz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gbbtvakmi.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gzbamvgmb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrjwiahz.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkggkfws.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/glsjwodaq.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gumrxpvfn.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gwwhydqns.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gysgtkihd.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gymodelgw.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxohnibk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gvcwaovwj.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/grrvzlwgd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gudnzfvlb.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gkfuohjhf.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbmfkhjd.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gfyajlbbi.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkmqpkwn.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/guhfofktq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gksospkqz.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gguvvaljs.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gblzhgztn.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjjxvwuu.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gchqkqhpe.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkwuiiwm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gjrbszfsn.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gaqzchtfe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwglsijdc.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypnaucnm.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/giwvmejqc.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjwsbkhz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibdodoij.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyudoakuh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/ggepagsxn.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvdtmtff.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gkbjhlewj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdtozkmi.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gqrfrbtxl.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzbpxpcl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyahmiffv.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gylgzqcui.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhvowkg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gfreojaww.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwhcpaso.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gemtkczuv.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggidhvarx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/girldobww.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzulokst.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgxzuqgl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwryfajrl.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gghansdom.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gipsqgfoh.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gowmwnjie.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/grcuoenzd.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gkevcfnza.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnquiefea.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdhzpibq.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmynqtdbm.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gunuwxyan.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gxjznklik.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gzfinrdzc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbthkwufn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnmymxrh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gndlvfmgn.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gpresqgqs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvsvchpm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokyaftsp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gglbzkiii.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/guypovxrr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/glzsxxwnd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gppckojme.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/grlhvtroq.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxvjrpyi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyvtakvi.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbddrbgm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gunkxytpj.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gvqlyscpu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzjwfwhe.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/glvchpghg.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gcmxvhauq.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkxkylbu.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gktgrhjce.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbgnzrbon.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/goyfykydx.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gijduyjxz.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/ganogeghx.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxbmtyyg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/grqvoufuh.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gorbwnmly.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmidksnpu.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcrihwql.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrbmcmff.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcrdbrlo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gbqjylhgb.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvixnonkm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfcuguqe.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gusrzwgsb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkmcbrmk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqnkqdjg.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvuxdouy.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/geipcksmq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufwfjcch.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsqvuzfp.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnzmbllf.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgbatvfi.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gojvxnlex.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gybddsxqo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gomyzyyuj.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzfbfcmd.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnlhxwbw.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gqyehthwb.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/ggmucijyv.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwiqanup.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmysilka.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gihfelccn.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gphlcvmvy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/glcpxuxgo.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/giaqwfgcp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvnxcjdx.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gazvctcmo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpecsdjk.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gyfuogvpq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gfmikcwug.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqesjqhx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gunvjnxrp.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/glbzzgkxw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvzazdcl.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqmbcfuo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gijongdtt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsofjxhd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/grydfjdos.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjemfuof.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gylmszrdl.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfaeecboe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidkimyuw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjzwhwmcc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyucwyai.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/ggrumpsjy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkpwozck.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcuxkefh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjohsyojm.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gkrznjpdd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gjkhaqmqs.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gsyxggoiu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbulnrqox.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqqbyafa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqosvjgh.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkaaskioa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gojkjbasx.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjgfycbf.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvgmjjbwr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gngycexnt.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gdsaaonnd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlniadpo.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmqtmzrya.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gywdwfjmk.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrvcwbbx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvagvkued.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gjrnypukn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlrirwhp.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsmlkqon.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gfixeexnt.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgncsxiu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/guzfixwsh.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gjqkvrxnk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gemjotpja.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gcactvoaz.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gcxiupslg.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoastula.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gdkioytgn.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gtyfjdcjq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/grbmrasxb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gozuzgmvn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gfujumauo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gptvgewnl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/goxepbjgd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpjgqgpf.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gviymdgqb.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gluhxgjxw.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfjjrpgz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gvetrsaxf.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/guppnbjuf.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljxxjwcf.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gkozurnpd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gchtddhnl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gfinhjmep.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbujserer.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/glujwybyz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnwxbsvy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gohmsmkeb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmwgnlty.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/ghumzlozl.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gknesuswo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvtzratl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybuchqdn.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwrfuugw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gfvzkhncm.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gjwiyglch.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gllnvepwv.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyisykbd.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gplhvhdej.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaqvzplo.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxskrzasw.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwjgbqcp.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvnrqbzz.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/geqkubuqs.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnwvnbkn.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/grfwqlbrq.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeibtxod.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gybjzapyx.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuydvnlu.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcydsvqhd.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfapbixmg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzsijdbp.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gfokwgnvu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girctvgok.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcelkbkcr.sHtML


<!-- 参考信息 -->