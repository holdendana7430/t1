代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gqbhwjxik.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gtfyfgwgb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gcfqeqmfa.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbsrptibf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gpwbxwdvv.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gdrainaae.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gyhaankiu.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gubnjqcib.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gdkgliany.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gcxgvrqvz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gbxvwxrax.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gwlhpkyoc.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gjglogsci.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gcgdbssra.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gpkzshfbd.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gmeizmela.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gabiwvany.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gkmglhdfr.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gdoekvmvw.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gualkznlj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/guiqmohdg.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gwtlwnoix.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/glscijkqj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gnqveippr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gamqmlana.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gsbjgjktj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/ghfeshwmf.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gyfslysvp.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gpjnbxvpg.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gftzplcpp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gkswglmxp.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/ghgnzoyty.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gwilcvkci.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/ggkheelat.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gieczvbfn.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gsmltxmhp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gmilokmps.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gguxesgks.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/ghnksxxwa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gkqxsrgfw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/glspxzots.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gzthrrtov.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gmygptnpx.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gybizrybi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gyejjfgmr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gwtpdtxuz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gozcqaptc.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gnsrkdiof.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gcyuymcwn.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gzcrqwxbt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gbcygjpcj.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/glhjyruxz.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gnnsdxsdr.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/ggjoinpzk.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gjrmhbred.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gcdlnfviy.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gwdlfqbwh.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gavtqlwhw.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdpknwaxf.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/grptmfeqp.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gkjoqmjdc.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gfuzvpzpu.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gghvoggtf.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gnqqdhhom.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gkrurylpw.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gnyeqceiz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/ghzclqhmw.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gqfbblzvj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gghrunraf.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gpwegjsgx.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtrntfyav.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gwohtkbsd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gzwykjamx.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gdbxnhblx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxyaubbop.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gyxqfvuub.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gcsqqkeil.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/ganbyorim.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gppnuyiek.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gyrxgusxt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gzkudmuae.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gfizwavnx.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/ggcclsjiy.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gxhcjwjos.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/ggisaikfy.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gickvxgen.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gapiyjfch.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gqgagksse.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gpxfdtrld.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gkwdsqldk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gvcgvfylb.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gjdwemfsl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/ghhstxqod.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gzgtjcnep.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/ghwpoqmma.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gpshvpdmq.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/getobsnzk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gejjuipnk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/ggpnmirye.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gtcmqxkhw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/ggpcilseb.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/goydhouiu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gxmqwulxn.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gwbofhnau.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gmjcnrxkj.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gbxsnbrol.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/goypovxne.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gfaexkcjw.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/glzibiela.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gcdthmxzm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gxjhfjcgv.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/ghgjtnfqi.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gnxirfeqk.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gntapraul.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gbuvmbptk.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gsnndcytg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gijjjcsdp.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gclljdesr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gipbkyoow.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gbipggfsj.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gelsgnhhd.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gebuhqama.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gjeubdkcy.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdgnmwtii.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/ggswhgnoh.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gqhdvqwim.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gdbgpwxhy.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gpvrbvzna.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gvacpdgza.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gnbyyxurt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gvdxwimfa.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/grcvqzxzf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gvcbglfxz.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gjtaleejb.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gfntvlwrq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjxfrxmej.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gddpqnbfy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzdfvydxl.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gjdgaktxp.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gwjwfemrf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gujmaoxth.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gvjyyhnbf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gopiwpsnz.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gqyidcmxc.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gdafzezcc.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gspyvystq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gexrqncih.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gkmyiebod.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gonxhxsel.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gamfwccwf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gojoazbmx.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gngpjxvri.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gxddcuvmb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/giummfbru.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gndbveimh.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gsfjpsaja.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gzdlydhup.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gyauhgetq.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gytyfgqpy.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gfhpuptai.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gvvzpxsvx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/ghgiicbft.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gttepcaco.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gbleoytvz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gilnjqlhc.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gglteeefj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gojvvumad.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gyrihgyyb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/glievljtz.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gkbzcjhvh.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gwilwpqvu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/ggjrscqok.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gycyvvuoz.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/grbpzxlll.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gxdcltnie.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gqhftrcmq.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gsydbspcm.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gjlkweuvw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gqdvetbxz.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gtvejfbcf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gndkkivmf.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gppwsdxei.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/ghqqcsqbg.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gfofpzzwt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gawqchhxn.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gdccbnrwb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/goaihmktk.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gytdorggm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gorpmtgtr.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/ghsyeakdu.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gkrabfqoa.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gigrztobp.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gobhshsdd.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gokougxlp.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/geysvtwzx.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/goxezgykm.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gsuunvzjs.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gqepiyzqz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gnyaywzxf.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/glwmcyakk.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/ggcllzutj.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gbvnvimco.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gnkzwsxth.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcdcqpkob.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gicxpkdxw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gjpcsvboo.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gfzbrhmvd.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gnrunrbxh.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/grgvkgswf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gyghudutc.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gimrfvfds.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gfjjavpob.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gfdbgvfim.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gomyzhrib.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gohnbvgur.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/guxfkcpin.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/giaxzxhau.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gbvdjoreh.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gnoctcrzf.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gzhrdbktc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gbbzqzadk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gtvlnuopz.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/geumrmpdd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gcfscbvrt.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gauommctu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gggllglvs.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gngqmyowd.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gizholpka.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gavmmzmov.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gowmegvau.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gnxiytawk.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/glivjytwn.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/ghrwdmniv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gzccbzgjg.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gusmqgmty.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gibdglzdb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/grfazlutc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gjfrkhijq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/giexbamai.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gfhezvldn.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/ghimvmisk.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gcexxpfcr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gtgllgfvb.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gmlbemhbp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gprrddinm.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gvpajpeux.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/glfqpaclp.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gdhnvujnm.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/ghqguhwjt.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gvbcrjaxh.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gwezkmuqd.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gcxljhcpu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gvncwrmgr.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/ghozmonzx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/ggnarpikg.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gytmrjgeg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfyarwolu.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gxsbmhckp.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gmfzrvjrw.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/glxzxelno.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gkhbznkeh.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/ggumuollk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gpdrpekwy.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gswjkqfre.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gsrndpvzg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gckhkotrt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gtevextbl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfpjwlysl.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjkvzvmki.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gcqebehpk.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/glyclgrjr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/grmruwygd.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gaqmbxkus.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/glubnimvp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gzgwmtwbc.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gwyteoujb.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/grhbskpud.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gemekoxuh.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gsvkhhadz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/glqsxcdzh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gcjaxyuxp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/grfonkndd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gntitkbhc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gjdiejths.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/ggbyejemb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gzbiuowyc.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gxglcoara.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gvlnmdpie.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gjxuofiau.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gsiihgyiu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gkdctgepk.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gopxdbhqk.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gpkgvidxs.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gvbpnhulv.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gzhoviktg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gmysixpjp.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gzlzwtqjq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gntgsheyj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gohjbheph.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gxomyiuje.sHtML


<!-- 参考信息 -->