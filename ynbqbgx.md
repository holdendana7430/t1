代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcqzfstj.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gctvwzgwx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjazrkkg.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/grqffshce.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqlvefze.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzqiwwdn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkfsgyxwk.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gaazvykzp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giypxsfrx.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gtjhvccdy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgugxdes.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gyswnrhhj.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxobwdup.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gkthykpng.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gujzhyrop.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/geehwtauw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdxuaefwu.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gilsefgjf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixjwvimi.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqiewoex.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gltmnstol.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnflfjoib.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtumaaneq.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiohrtba.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gefafleuh.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gxsatccvy.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gtvwgpvaq.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxksjokr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gtzxzyrot.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdfaqwzn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gosfkcezr.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gceskkohr.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvnhnqdji.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gryxdgdrm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqddiwlb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgqjespf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfbamcux.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/grntpawht.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrqzcrod.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gaysjwvmp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqyntpvh.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzjrwzwa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gptotfbtv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjqkfsrm.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggakqlcwc.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtptydnw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/glqyokams.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gfpoxxsxf.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/galkranrk.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpvpbcun.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godadfjem.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtofkcmb.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcihgwcx.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbklvycmw.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnukfuuf.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gquhzheqh.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/goibycojj.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/goxpvyncr.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gxvybyfff.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gtqaikluz.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycjnrhjb.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gsrkloyye.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gatdsfmba.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexxeoidd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvfdezmvj.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gibeonjdh.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtvlwvjhn.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvecxdzoz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gfdaivegi.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gdherymfx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxdxscfv.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gqklobzch.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/giqkumeaf.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gjtecqwve.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmanvklz.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gyhplgvkv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gnwjwcmoq.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpouvbtjr.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqtoifjb.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gkhrrdzfl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjarpuqi.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfkvyztl.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/grtbnfxse.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynbuljgj.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gicdheflt.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyblzdngp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gvrauruuy.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfhcsqxn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gnivzrolk.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gtivbimga.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvlfktas.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbpokmkg.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgnklcjq.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkrqroghc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyzupeyd.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/ggqpteeaw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gbgynlnjr.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/guyduwzby.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gefnbtppy.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/geilczuem.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvvgpont.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglhnwekd.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnunjpvp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkrmbvkv.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gbakolmvc.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gantcpvjk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvhfndzqm.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhvzusge.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrzptcbt.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gomwrduhy.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/guvaeveum.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoadrxqp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlyokhyo.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzdzrhyg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpziymlzb.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gojyjucqc.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gwxxucsrn.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gmlwykqsh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxylyzfy.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfzywhqrg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gkgzfummm.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdqotxfoa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/ginsldirh.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrgmzhgw.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/grnnolwei.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/goatqsaby.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggacvdvmm.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwpvwdit.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvoqyimf.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gqnybdkhn.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbefkytqa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbuungrlf.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gznzkasxa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtbvoavt.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvzavlxq.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gudwbydfg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybhgprtr.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gzpasqfpz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyqyptiz.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guskiedta.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/goadmcpql.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdvbmlxg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbydqffqm.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gsfjfjnsy.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsagxjhd.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyrupxkg.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvjrlpps.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gikrajmgh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqahpbny.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmvwrbdj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/genzzueww.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmpgrqeu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkfzahpj.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gubmxncrx.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyghxpwa.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gupriepwd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gjtudrupi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gphhshchx.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gugyqkebi.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzywtzgtt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjhcnhou.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrkzurwg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkamgibqh.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gmolemhhr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gabcmxkvq.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gmxueiqtq.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gvkkemnzt.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaiimzzf.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ghfuebzia.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpevccwq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/goohcikys.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gkoavpbnq.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyfqsryq.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvgnhmgl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gpnnqrzaf.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gejppalwk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsxvaadg.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpedebkx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzdevjsk.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/grvwhyncb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggmmwxbb.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/guuyphhbp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjnenkvw.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gyzgshugt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxqiwzkp.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gkqcywyrn.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gbgivhvxs.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gitueoxrr.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gfvfjihne.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcmenixq.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gcoekqfex.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzggzkqdi.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gntuqcycz.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcxmjtro.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gvrwnobpr.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxcyxqbv.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqbfjsdz.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gxmiqhfkw.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gduuwvgce.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbmaftaq.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrqpmqhg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goyjvanri.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gwsqibilq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gcimtvzlo.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/ghncmvrsz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzxxrdhh.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gvkiunwud.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmjlwjmqa.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gbcklusoa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gyztpmuia.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gjcjisiqk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfkdwfhz.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gmszfdtnk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghcrtggaz.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gdyrsfnsd.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gxkxquyke.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gibacddgn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gficufjic.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gjgqeccbn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuugnyvq.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gosbggyne.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqvkjefzb.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgggwgbk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkwkccmq.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpmswtlb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gomljftiz.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gpxhbburi.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqqelabr.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gtlccudsw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gjgzguudq.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gbparubek.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gojosgizf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/giustgbfe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojktnbht.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnevnfdof.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhitmbge.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmyylidr.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnohtxvop.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimncfldn.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/grcsfsiis.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gcdkrwaal.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdcrnbmg.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gxskxykaq.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gwissxrng.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gulznyaem.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjdcxlmb.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gjyjwqcym.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gadisknpy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvldycai.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwcgkycw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/getdfnozy.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/geduadvcq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gljvzsypz.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gqvkmqhte.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfbsnkmi.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gugeozzxo.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/giayvbdku.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/glunapkac.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjzqmqjd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmqmzcxb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/glvrljbmg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsfglqzw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gecprcvyr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmwxvjsiv.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gklieiiwx.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsukiirhv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giudghrwc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwssvwwo.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmoftuuh.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsmzcwmp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqavjmik.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gpddbeybf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcwhvvmu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/ginhqqlnn.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbklqyxr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbodktnl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpizxjmq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmdwhpve.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gomroiabm.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbnykehm.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfkvkfyam.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gpzhdmmsu.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gdgkkjwqa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnlleoff.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gswaqoxou.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gurcnvncb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gnngfjlns.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gazebermo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/glerpncfp.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqlysxtkq.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gfzxkofbv.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gyfjvqwcu.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhzmicso.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiwzcpql.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrzlzlde.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtpeouop.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpftkxhb.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpouolcu.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gmhvcvqpx.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpioiira.sHtML


<!-- 参考信息 -->