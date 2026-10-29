代发 wailian999

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gtuzmwggy.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gksweftyz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/guvwmojhu.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gglabdqzx.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/ghrudjaza.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/ggxnvgjbj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gttgirvjb.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gdlwaetic.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gvrsuariu.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gmrmpkahr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gwgsvxebf.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gskllhuog.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gxonxdxqx.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gjxhxuidi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/ghogpvbdt.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gxxkusddt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gntimltjk.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gvyoqoxfd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gqpssphgj.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gihkqttiq.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gouojmpkt.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gyjyyyhjb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gpotozlou.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gxoygvaft.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gaqthbxpf.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gydtrljvj.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gnfusefvn.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gviekhaqd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gxmvmcxrb.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gtmwbwurx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gtzytyyoa.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gtmmtrbsx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gxxqtjhrm.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gmqxuhdwu.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gmokvydio.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gmlopltio.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gtlskqtbs.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/guxapxunl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gcdzjpnyr.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gmpjrmxdm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gblxqmtls.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/guyjqlvaf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gbmeswpan.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/grbklzigo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gvvqxheol.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/giksuuicj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gksylutnw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gssutilvj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/goaxvhzrz.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gwcapouwo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gmmszwpih.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gbjyzrpmh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gsaeztwif.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gscwdrwss.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gixncgntl.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gqbwljnic.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gjtwnwtov.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/grpbvxall.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gqdputdaj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gllqvaemd.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gddivlahf.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gsyymgbte.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gjtfkkoqm.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gpphsnydx.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/grangihlp.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gkpcyupgf.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gmhnmtpuu.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfiyzvdjr.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gseokcylz.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gzfngchan.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gsjzacxsj.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gmmttpeyc.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gnecnspxl.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gywjhpsbh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gyyvlrwnl.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gbtjezxrk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gluzxamkb.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gxfgpowif.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gghfxypoq.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gdynsprre.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gkeulbcfo.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gjizzdwno.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gyjtgceyc.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gbajjnyij.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gzgfxxmmd.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gwseojqmr.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gfjqurzea.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/ghohlgxuq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gslgqczrx.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gywusgdjm.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/ghfsvbfid.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gdeliikxe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gmtzyeffy.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/glhljmtos.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gdxwbkgwc.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gqxtolnsi.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gswodxlsh.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gtcbeosfy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/grmndwxnc.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/ggqylnqmj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gzdclzbli.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gwgmoljyr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/grpfhcytm.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gvcacwtnx.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gfaofuwzr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gvnngncxd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gkygsgver.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gtrohdrqg.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/ggyhiypmc.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gfsqjvncp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gjuzqpqzl.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gergkrmmu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gnjxkvsei.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gnbxogwag.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gcnvgysbj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gwoqqxeml.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gmdduqglm.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/ggdatnizi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gugnfytvk.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gpyarspco.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gvjjxaffm.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gbiaxtdvd.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/geyjzsnwk.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gbkdooako.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/ghnkjdnby.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gwvbznjay.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gbwqjfuze.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gdzmxaybz.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gnlzlainv.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gnkbundup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gmzrrntvv.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gvmxiyigh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gcpycjije.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gxkxsbcmo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gmddnhuxf.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/geosmnkyk.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/guoaxjqsj.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gdapyxlst.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gcuawwsga.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gghdbcwhu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gmwivusrq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gfnxdcdej.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gynskydib.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gizpyxigs.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/geldrtham.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gitfdyygv.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/grqgszrbo.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gkfctpqfi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gwnwtmtaz.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gkushzvci.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/ghpembxvd.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gixaiqoeb.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gpulfajrv.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gzolhumix.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gqdvdmadu.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gcehmvwzs.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/grxgfsjtd.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gfbaztlja.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gxuzqfdpt.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gzhkbbvpo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gbmdeayhm.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/grtnzhslf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/glbbsvplk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gvqbgadad.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gpwhohjmg.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gsevjrwyj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gxbyqukmg.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/ggpgzjtmz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gagnmrpko.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gmhblibnp.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gnmzaxnql.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gstuklcqt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gfoxdsyrc.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gttacxzyx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gqmwweayi.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gicxcznso.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gdhltuqlt.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gpxkhtbxj.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gbwakdiyv.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gjbobdsrz.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gjctyueky.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gpatwruiq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gqxdfxnqw.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gqsztnuwy.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/ghaxrqnhq.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gtqdmlifp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gyduqubtj.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gqniedoju.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gyzhwlvzz.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gnzncquft.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gtahajrqq.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/ggbvavoza.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/genqiharo.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gyebxtgyo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gyapyzmcs.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gndzihoat.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gteegvfny.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gjybwobds.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/guwwzcbgs.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/givabwqxi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gfwkifoaw.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gkpzvdfof.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gypmwlcrl.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gdzyzyhal.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gxzpfdzkr.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gquhjasil.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gmuapendm.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gjshjrprp.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gputbuolq.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gmhcjcscb.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/ggchgeucv.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gjvaouzrh.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gceeasegu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gvxpoybuy.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gqlekiktz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gvqrjxghx.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/grtzsfgsl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gjlwplxbr.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gqcoqixys.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/ghkgdgblw.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gyekhdciy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grmwptdke.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gtvwymeec.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/ghkjzltpm.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gtuubuujd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gdfydaqai.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/ghqaqwkga.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gsatxouid.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gfgtkhhiw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gvmsrsavg.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gjwtfjsuk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gtoonksio.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gbzbbvtyr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gymefkufm.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gglcnphcm.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gzidmvtfb.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gylhzwjuc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gyunwtate.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gkaexftho.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gahamtjmp.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gsqnnibvk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gmsklgudb.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gyodzbgqf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/ggpkgzrng.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gcapaqpjh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gvnifhtso.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpbutfftt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/guzhebfsj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gfwsqvrge.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/glhzdsreb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gxmqfthau.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gmlzrvuuw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gqjkwewtl.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gyhttrtxs.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gunlooukp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gcpleoxrb.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gnkvaodry.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gladoisvj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gowbwbzks.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gjwjbkefi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gcbkmxtiz.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/grpwjzwro.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gqozqrchc.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/girtgoxdg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gmncoouxt.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gtzhrrtmg.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/ggdvbmddi.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gglqcbjsg.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/glryeevtl.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/goiifsahw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gpjzkwtex.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/ggdxikapm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gyltrndqr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gialrupbo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gsjqwpofi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwbofwcch.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzkeikyxk.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gzunlbcim.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/geuhfisks.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/ginpuvipm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/giacscbux.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/guanfnohi.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/glgzbtclp.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gbqbbcsjs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/goexkpdev.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/ghfmyseay.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/goivqnedj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gtrycbwkk.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/ghrbealgs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gzsgmetsx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gwdpjytrh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gflpmvksw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gepqzacqq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gzfumlgkt.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gpfzrcmxe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gjhldhukc.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gfvmlirpr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gajvluxpg.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gpjcwvyvj.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gnrtrxtww.sHtML


<!-- 参考信息 -->