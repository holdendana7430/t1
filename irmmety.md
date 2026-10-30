代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcanrzgji.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrifzype.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpoxfvkyp.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gydpuhsxm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gplwjaeig.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdinddoy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqtwhonr.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnxyoaza.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkhnxkgp.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/giixkeycy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpuyeqke.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gderrekkf.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfsbkvytb.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdmmsmhp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigicpkmp.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtmjoptn.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpxdjyhkq.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/glecdjlfp.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwixbxftz.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwosxasp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gdizccwtn.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxjmktzz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guqqyjabk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqchgxfj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsbvuexeb.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfoqfuclb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/grmxrfzpe.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gkndpsggt.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gnoemxbkr.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxrmhdgs.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gskevusxs.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxphmlzwx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gigsrbreh.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gtqrwgpwg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gjkcfqucp.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqjwemxz.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwzwuyfd.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkzqlare.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdiqcmaw.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gidwntpal.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gjxydpcdz.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gkibvdkrk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjzmehmf.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/giudrapuk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gfhltxuhk.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/ghfxegcfb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsewaauj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxetheis.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbxuhcnry.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/glezvmxqu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsjgeivk.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gjolbaqzx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpopildlh.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gpliunnbs.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gjqqoidlw.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glazenpde.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiuszzth.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/garfacrax.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcxvhjrin.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzbqjexi.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoarncmn.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gewypvqew.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gptvjkoen.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipgektik.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gjdyftcse.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeqispgw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwermhuh.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvksbnwze.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gslxorqfa.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/glvysmeci.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvehnluc.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gjuooudxa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gundqrbqg.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/ginpunrma.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtuktylyj.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gkakbqxtr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/grqvbktqs.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gfuanjqnt.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gscynmpva.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzrghrjr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gupdoiftn.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gojzxqttw.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtfvptjw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyxefhbi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzjrjltk.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuyqpcmr.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gfurlzisp.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gybmptbqp.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gcvytuqkw.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwosuuxxm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtppjmyma.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdhbfoel.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/grlogzzpb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/grlhkdqrq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/grnjqtuwk.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdidpqls.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gchqecwaj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsvjqneb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwthjrknl.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gurdgxcnb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcvmhyju.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/grpuqpate.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ggpbliydq.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gqptnvcdh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/ghleiqotx.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gdzcrmupz.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyzyaqqm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gucbgiaop.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gjuqsmblv.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ggtgsgtyu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprfnnwuc.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkmdeqxr.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gdvleluyg.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqxvmkoa.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrntinkh.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ggaaguhjr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gtpqgppuk.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gybrezhki.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnuorztc.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gmodxhkdx.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/genuqzxop.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrvitjlx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzbuqmzh.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gujhbgktl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhbadvps.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/goosgonnu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkwvflni.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtawfsqir.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqqhcbwl.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gnncwonid.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghlipxsrg.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrmvkfen.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmwcyavbn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxlwxukr.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/getejkiul.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfhqwueal.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gsemityar.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghltdlvim.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqscbnspl.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzmcpbaf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxnaqxdo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gdzhvnrrr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcqizfnz.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gabcxcrfr.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gwwughref.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/goghixjmg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gynogzppz.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdypkeqs.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagbpsqrq.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gbanuvyhs.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gunytdisp.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouycrama.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gkmgxxbhf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmpbfmdz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgdxyhws.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmeoaakz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpaqojoa.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsxxwgaz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmpfvhmv.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gktmcbwfg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gefepmfra.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmlzhtbn.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gocnraore.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvvutxqmj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gcojjqjpo.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gkiayscxk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gcxdbhylb.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gpzfpoomm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzvsipfu.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrieppnj.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gpdghecnf.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsgmyofv.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gadfjvgzd.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzxywyhw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/godzkpixf.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdcjyulh.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayfobgdt.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gmlxzjips.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gypvtjcvl.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gydoicpjq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gjitnfkja.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gjyoiouyv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfcpafqg.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjjixtfz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjfexlwg.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzkmffky.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gofmwtoax.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gxwasftwc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gzncpgrpt.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavgtlgqw.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gpqahmuvj.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/glcrozvkm.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glidmhcae.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gefswgxsa.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtdutcly.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gluswyedi.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gwywprajp.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghdprianp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gxtdhhisc.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/grwvdcddp.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gqqawgskf.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxvfkesj.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gmamoalik.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxvzjctog.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gdiyqibtk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gicsdfuuf.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlpqxnju.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gkzzievsw.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gihlbtyki.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gmtsrmpbt.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gugauxyym.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/guljiniln.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkmxbbxy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpgyjeih.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gerqzwrwg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gefeoiata.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsheytpb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmttcxrvw.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/guxribjmr.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/ghidxgjtr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsgzzerk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gczzqjnmk.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gdotbdlvs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrjbcrus.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnwxmsosv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgzadmly.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkvajklbp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gclkmwnsg.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/glmoxxjsa.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvlnjfqp.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxunvpfg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwkneetf.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gxrcnkgfe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gqicspoqs.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gjlzlsorb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfzfgotg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyjsgpiu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnpyqgzve.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggonxtuvy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/ggabnowmt.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gceukyfgn.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmkaqrowa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/ghslsdznc.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/ggioevxol.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxduioont.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gglgpmets.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/ggnyvnzen.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldsklrjs.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnywmzrya.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gkquvnrnw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkkzrncy.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbgdohmn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gzgzerinj.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gevycevbi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdskifezz.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmoxwhyb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsyssmvis.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmuxsiiv.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzxhnwym.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gyzevrcni.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqozqxnyh.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gbmxttjej.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gtawsfken.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/grngdzvqp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gmqevtxma.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guuyxdwfe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbmbpbbb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkahpzcos.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gssrqdbad.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbpzvcvc.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsbxqapfn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gzsartcfp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gjffkakwj.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gutueblqc.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxbegvnb.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/ghifsryzn.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gjcczaebk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgjhfzgm.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gubqplcaz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabmybpef.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/guzvrjoec.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gsswgwsee.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmmovyoc.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gajdjashd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscgitxuq.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gewzcuupw.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/guzxfiwsr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gvooyichi.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/ggekysbth.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gjqkhcacp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gobjtltid.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnlcmnoet.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznmnhpiy.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gvwvisowb.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gwjqdjxmq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goysiajzi.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcvvmdrq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gaeomsnoy.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrssypfw.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbvjrmjfo.sHtML


<!-- 参考信息 -->