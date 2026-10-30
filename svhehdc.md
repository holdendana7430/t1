代发 wailian999

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpfxuses.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkykctgqn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjahcjyjl.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqhaystu.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdfsfhpw.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxnhbgom.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gytqhqzkp.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfpiqodr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gczzmkhni.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkofgizry.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfhwtcjfc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlskfimg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwbnzvpr.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjzbhesc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaudayhaq.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbqfqltr.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulbnfirk.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gezpygtgt.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtzpeglv.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/grhrsiiak.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkqjukfu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgkmoznl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqtejuoz.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkwgweqg.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjagljuaf.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gprecahea.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwmklniuk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieuxkwde.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfadfqdr.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gvcylldpv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplnhhtyi.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gnijgrzfw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gufahzmrd.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtemrthjk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/guadeuvgr.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gevzzrvwf.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gisxogomb.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gomlambmh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpdqonkx.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/guacspauo.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gqcxfytan.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtjkqnwd.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/geicrlgta.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gaetemomi.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gandhlglq.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbphldbm.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guvacwgzt.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdnttutf.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gikpkidvu.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhderfun.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gtknhjyll.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcnwclef.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyhaoayz.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gyonwazaz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gacfzikip.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkkbzrelp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsogcxosg.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrdojtar.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/groncazrc.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjknyzol.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gknljdtbt.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gvtsnqrkz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gucnkowzk.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqxszvqr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/ghuajroqp.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gavdcyuda.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjudbplz.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gilvdpguz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/guattacze.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gujvgwjxf.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjububbc.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrabwysl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrokjnsz.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqnfazdz.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgwofwpc.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gxvldofha.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrsulagv.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkprghkqs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/getrwcyuu.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gihjckiva.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgyewsky.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gtdjcatxr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gfacnbpew.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmcuuqog.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvqpkkyc.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gaouckfxz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/guyppbnql.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkcbyqvd.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gomlreejr.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjztqbsq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggshlvxis.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppivgpxw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzvbgwnz.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgzejpdu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoxcnlii.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxzraptj.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljwgylup.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/giguvyhbn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbvugwuo.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspdydlhk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gfeusinoq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflllkalf.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gozmskctj.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gajzyoiau.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/grwjuprzb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geidugubb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqfrtazg.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gfkleisei.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gvgaqijvj.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoufijus.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/genbcqgda.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gscjmzshs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbekormyo.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpcunfand.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gjlbfsmhf.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwxofqdq.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbtrmivg.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gietxatta.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gctctoixa.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gadcpomsb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtypcozjz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldkzicng.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwhcuequ.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzoqwzoft.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/guhveokmx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwsxqfrw.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gncgprsri.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/grxhphkad.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmijpmotc.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gddemthhn.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gjgijvinx.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxwdyehf.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/glgtsvbml.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqupdjrm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gdzchvqwk.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gliihecqq.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqtseloex.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gkyktxvyc.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gkhyirtoj.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gioechtzo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcwnpwjp.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpqxlooq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gkgnjwtpq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gawgajesw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgmlwooo.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gvwtfsyke.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gacqnrerg.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggtijzwim.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuqybtiq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gyiziirkh.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwqzoufz.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqwwuqhve.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gagwvexlc.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gejygeuch.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gubpfujdj.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmhnwbes.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgibrwlk.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypfxhbaa.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gfhbcettx.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/guridtiuu.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/grofwlfcu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigdidanu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpxxkwcz.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/glupneihn.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gicgkwzcw.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqdroydp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmqdimvr.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/geaotzbgg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrarezjp.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gqpldgktp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqalmepqk.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gwvwnhblg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlvhtezm.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gzaasrnmt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwblhdaaw.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gkpjxttah.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwknpptwd.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqhtdcbc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgbikcra.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gpeahynzp.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gmfnqlgrs.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudnnprdi.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxluahsm.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnipcizlk.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gibkhkvst.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbskoaesw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxpzzxwh.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gowwsdous.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/geehxnrmm.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylxcweeg.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkpgvnjo.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwatdessn.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/geiruiwir.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncjiywbf.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gahbxrxkc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gofefuvcg.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/guyyjdicq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfkacqsm.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gbekhqctm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbihstgd.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gzxcjlrqv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwwrtzece.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjgjszwb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gunybfrqz.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gioyssoux.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garltatir.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gusfgacxh.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/girurqejf.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwcstqswu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfelvbzkv.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gqcikgvev.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvupdfsar.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmvjovmxt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gsheqylao.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwhgjupnj.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzviilyqs.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gjsrtzdik.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gqpnyfrrp.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmewftxt.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcykdadqa.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gwszrlllr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzfmekqm.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gjosfaqoy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdzdsqng.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/grqgqdwtz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxbgefyy.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdkopowy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqsbuqwl.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gkuakkbbh.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gndlthnka.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gwgqmveol.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwedsrpv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnzjikti.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gnlsjlxmb.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gcefxnbpg.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gazccjjmq.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjhvjfqy.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gvenoblce.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvwuuxfa.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gxihngrlo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyovhqfdm.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gyhyhbsmq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjigtsrza.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbwbirko.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnqipsyo.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwohmykdv.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhnvgykn.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gkbgomajs.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gxrswohsh.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuzryoqr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsugfspdu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbhqqbgy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfycgwwk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmexelto.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbdqfwwb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaiyiexw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnlykysz.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngpuzxnw.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbncrfwo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gahzracqp.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gbhcjppzd.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gnzgrdszm.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gyormmrjy.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdeefyiw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhmfkslx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gfldqftoa.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbtanyqy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqadnvox.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwhzqpoa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gerhlfkwq.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gskbwsjxg.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gicutcwxl.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsguwtcaw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbadxmubz.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzikkfsd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbqwlkxy.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gxgwqlmmn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/grwlaezvl.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/ghzwgqdwy.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmohtrtvg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsfjbspi.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwuswxzej.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggvuffmrt.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gjidipjry.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gxobuwepe.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneyomkpz.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfcfccavl.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gicavgpwp.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlmrhwca.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghozkrvdt.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnljbnjam.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvajqgez.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gunoynplj.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaujknwi.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwkvvhpi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gqvcwmbsf.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gasdetrfo.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gkyjkrkic.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokzcssfi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghiockoel.sHtML


<!-- 参考信息 -->