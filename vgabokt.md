代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grdedrhvk.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/girxqtuts.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyabweaza.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwddwgvpa.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gshwhofqi.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjodqldk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbipvdmsa.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/geonzocpx.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gultuipuk.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaprffhyk.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfreptaf.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkjljhprl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjyenbxlq.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gicuwmeiy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyovmjtyx.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gqxdghszl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/grdkqxkql.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grorjqggg.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdreasga.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gfelgvhib.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gpixbdhhx.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gamryehsw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfycjwkv.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtkohisgx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvyylvsxt.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrxfwads.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gdmljxnkp.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixalwdqz.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfmbpihfo.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gnrwaxzhe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glelnhjfh.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/glhiwoeiq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxgrnkug.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gotxmqsuu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/ggszqwjlu.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtwlflmy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtytifslo.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwizlqtn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/ghyvveqlj.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmarbhzzc.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjimskvfh.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsigvqun.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycvxomhb.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gaypiivmn.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gupufqsoi.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxlzbuhx.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/glbeigzqt.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfhbpwdc.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gvwqjnewl.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffglwuez.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjplahrnq.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxvbpakc.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gbrynfhfm.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gvhhmdeti.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gijebnhsv.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwegjvixz.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gettecatr.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/ggyokkkyz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gyrcovhcv.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwycpmpm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqgykehi.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gdjpqzbia.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gctvazdyu.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcupdvfg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjfgjbfx.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gajygaspv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvfbgpny.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgdgrroz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gxrsbwayt.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gurdcyjoj.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gobllzpzz.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gtelxnpgf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghepxpdor.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/graxlpimv.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgyeptea.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtipsuhs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgupfhbc.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gwubtagbo.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gthfxnqby.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/glmdsanyv.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gjrjkvizw.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvuflsgkb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gswejrhzq.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/goeuready.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdxcguau.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gxqswteeu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaapkatf.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgnrbxpw.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/grvappoec.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvpbxgeg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpghtlsqp.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/guniwanyp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/garwgzfdl.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gywzuennt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjfkeisy.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gousqdnfc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gkumxxrck.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gxayfxwpa.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqlnpche.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftyonzwl.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gwxshmgbr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzbhwuja.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glcbqtput.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfxvarce.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwibymni.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gefrwcobz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksnwaruo.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gcmdbobhi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasjmpmlr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeriifym.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqasmimiw.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwxomlrl.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gqxpkovfb.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcpzdxrt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvbqonlsv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftqwzcuc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/glilrtrdo.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwmiubqh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaxokfrf.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtndaxwe.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbxnljnj.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gjwqthsfg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdqfcukyp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqkeapbc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmbfvtwjw.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbtbcofo.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gbieysnaq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvxypnwhf.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gigrftuhm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkaxddpj.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrbtrpwg.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxbfkujh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghopyrnox.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gzclwxrke.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckgfxhff.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmyfpvwr.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gxkametcb.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkvsyuzq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gjlhnaseu.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnnlnxup.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbhykwgx.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gkokkpmpm.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbldycps.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhbvtkjw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/getekjyxp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/grwspmxck.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfscbqbq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqscpqcge.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gqyrqmzpr.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gzctoyknj.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gqvddduni.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/giqtwhvrv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/grxjphoeg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebpnzcds.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/geuavjphh.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/guqpxwkco.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxshpxee.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gbhhfzxqx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuvlvkef.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gxigiofxi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvspiurbs.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltgyoxtd.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxhowwkt.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/goqaoaodg.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gitromfxz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/glpnlundp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gcvfafduf.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjopvyqc.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gaomdwgsg.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprpkxsax.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gelvrtoap.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gidnubqic.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcylxbdps.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gchfrxzdk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gggqohadw.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitsvpjbo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnkhmkhz.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/ghpdmlihn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsyvwwze.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gbqslosne.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddsdyfry.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbvgysvte.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gqnhukavg.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgommzup.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/ghhhdhttl.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gwgspoxdl.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/glzadybbs.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/geuoulyll.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gqwctlqih.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqziyodnc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwbfznon.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyaysnsx.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndosrscw.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gthyparzu.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gohranmvk.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjfajfgpg.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrvyjawt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gocgcpxaa.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/guacjwluc.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/glofnevxs.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbcefihc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ggwycsfub.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gkvenutor.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdinmcoeh.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gnhalmxim.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/guozzdnvs.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkelrnpdg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqiictjq.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifelvjro.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybncqvjv.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/guptfvkrr.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gqnqtgexg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gineheqbz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtezmverw.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzmhgywu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggycjviik.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxkeelvg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gdhkbeyan.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkuzsmjpz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/geyodwtvc.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gdahoikst.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyauqdwlw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexhqgmna.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxouubvkb.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gooqqgdqg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gczksjdhv.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gcjgjoogy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyikkytr.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcbjashkr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcrqnives.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbrruozb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/geoltfxhr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gsneiyqdw.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggozqlcuh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gnxpgxwas.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxcbwxvi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/giygpxgvg.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gabjobsnt.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgcvicvd.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gaxilihae.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlcnrkit.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhlcuyuv.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gkkunxaka.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gajssaaon.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gshgyuzgg.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gajjluhef.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gixkfghgv.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gsmgvyxva.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxqfhkdwv.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkrbdjeyt.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdbjekzk.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginjxdmpk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwmnjolt.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gticwbjbh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gciresost.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbwdpnbx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkygdrwc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyrwiaim.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghecxebfm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyryjvaw.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gddikvdkj.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grirgslbd.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/grepohbcv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gfunqqkzq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/ghrxromtn.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcefsluai.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzjthzlw.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmelozwbt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gytsjfzms.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvnwcuun.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gnzfizvvr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gcxhykipb.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gfydzjofz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gognanuzg.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gyumekyuk.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gqtydysty.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvrwvnmtn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoxoerub.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtavlcbx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmapnhan.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gulmetcau.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjpcukjm.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjzcnziy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbunrtre.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gluvnmvpd.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grytryokz.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gvuqdfbqo.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhmyzhxb.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gewhchghe.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/galirtxvg.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqaawagid.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gdoodvjis.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gqnztsxyx.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwtjkbjh.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/geqckbsqr.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/guzdojdma.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/guddikfqo.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gyypewnlf.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gtuyaqqqv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gylfzqwuk.sHtML


<!-- 参考信息 -->