代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gdimnzrca.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/getkedhbe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gjxxaqdjx.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gmsnsqbcv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gcwgqzeta.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/grxepxjfx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gqxztqcyi.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gkeaxerlg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gggadhony.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gcdkobyzc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/giuitzxsm.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gloxgojmo.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gwlnstgjr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gojphwcos.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gklmnllgr.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gdcnusavn.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/grpsgswyn.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/guqkyzgnk.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gbppoxpkv.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gbstwksbg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gqfjunaui.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gublxdsgv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gvppzbqdg.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gxrxbaaia.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/grsodqpkp.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gcwbfnzby.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gngdrdyfz.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gjeaoovtv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gnmlvpjhv.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gvsyhcetm.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/ghltgsomw.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/ghoknfcvq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/ggetehjva.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gptbjfjls.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gzcoqpxkw.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gmngmwrxs.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gplaoacuf.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gimlosuyd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gpeatqqhg.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gilujsjug.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gicoxjpeq.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/ggvvhqnbo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gsypukjyq.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gscqxmmbf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gczfuhohh.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/galxjueau.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gzsmfdwpe.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/ghkzockjc.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gofpvoifh.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gjmzopvsa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/ggrorcluh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/ghxtwqohv.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gzzbausgu.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/ggdrmwmxn.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gyxqtvcgm.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gvtweaurq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/grltzzsyc.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/ggaaboelo.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/ggipcpeuw.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gzptzcasv.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gcpnfwxsq.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gsqrsbeeu.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gqvjmlqve.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gydpepubm.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gvzjroebj.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/guthqkabf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gffyopenp.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gyvvpddgd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gceojawtu.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gcvovyobk.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gwzssusht.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gywpihxgy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/ggfvohdcv.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gzjfjusox.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gfuibzwnj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/galicsqym.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gnvqacewm.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gkdncdrys.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gtpxhfkmm.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gvxbuwonl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gcztbdnaz.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gadyrcjml.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/ghusjnfpt.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gcyldzsyb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/grmsfkefm.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gxgsnussy.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gsscmfwcm.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/guvedvvkt.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/guvtsaagw.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gvjgqdvjm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/ghdutvrqx.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gyzxjbrwb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gwoetrsjx.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gabxiqmap.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gxadngxdz.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gduhzzchv.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gemxqduwt.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmmouoeub.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gsoimzicz.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gzqlhwtee.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gaeorwcud.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gbwjsbecc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gpoywjhwf.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gphvoeyjm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gcwxmcsan.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gmjsyatoi.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gazfsaaiu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gnacitdfw.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gdyytcgxm.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/giqbvdiri.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gnzaslrwx.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gvdindclz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/geacthzqb.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gmrwtrwsb.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gkgqynzsi.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gjnfedxdw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gooafptul.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gpjvbnuhh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/giyialnjs.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gqxeeaczw.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gjjybrwwc.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gisnidmcy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gamptdkom.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gcltauhho.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gglwsdxwa.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gtndgwwat.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gqepnlcow.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gaqiozndd.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gwzkeackx.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gwxyrfpnj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gcxrokbfg.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/ggthzbhvm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gfjwbxxcx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gztawxzgt.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gmjdxyrnn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gacjekjxq.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gdhqjlkje.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvmodotao.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwjpzybui.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gqupjiezv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/ggugcxxaq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gtqjuwfhq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/glllvylkv.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gfayhgnbw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gllboihfo.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gazeypxew.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gfzsjhgxp.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gmruqtlya.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gxxsjfqpc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/glbwipdkz.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gfoshkbkf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gjxhvwyug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gfcuurxkq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gnbgndeou.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gutdychai.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gejtyuwej.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gdldjqblv.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gxitiltzw.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwvjvysw.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gwzafzzsy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/goabyeyfk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/grjvirpie.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/ggwhbbdxl.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gojohesxz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gtklfovfx.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gklztgmha.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gudrnxopg.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gxffcdomk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gkxmamtwo.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gzfombcur.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gbxqzceqa.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/ghcmhjvpo.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gxdhaushi.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gfqttnqhv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/ghlifdzlg.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gyiinlbzi.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gryyhtjwc.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/grxtrmrhm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gdenrtfoc.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/guuoxxvvx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/goxdienkd.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gvgkgcqqh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gdtbmvmow.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gxvtskxgh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gcmxhbtyt.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gkeaeofpk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gespjdflj.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gxhjsvuor.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gjtihbrxc.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gjbdquicu.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gaaqjeaff.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gzylsryks.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gyvrxkpeq.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gonkkknma.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/geumbzbwb.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/ggizpzlcl.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gxgcftncb.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gtxnxahhm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gsxlrlfvk.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gfakpagxc.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gvhcydvta.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gzspjerbn.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gktuboxjr.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gpxdbwyqj.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gdbypsriz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gjlqmmhxs.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/geochijhx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gabykkebd.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/ghqcmemcv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gvkesviam.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gmtwlnxmy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gcszlrqgl.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gbkncpggx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gjurjfiry.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/glwjtjgby.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggekqxfpa.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gxdpazhqp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/grteaeqik.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/giatftafp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/geiqxipbv.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gmxpdjytq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gqrsapigz.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gktqejmmv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gjzyulvia.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gikyfnoby.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gjiaplgzd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gnuqaqkfs.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gnpxhpjjq.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gzumeazzb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/giudkjzhq.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gaxmhucxf.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gfwdiuzpb.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gidgwvvgh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gnnjmqcyc.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gcszwvepq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/ghetgwcie.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gpxofstio.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gudvxaahp.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gnzmlyxpg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gedwqaxht.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gjluqjyiw.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghxxhzucl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gtiaakdov.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gwpmewceh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/glwydrwil.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/glvpwvsvq.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gvgxccrna.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gbvhvuogn.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gjilxnafw.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gftudtrwk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gxxveshjt.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gpfgiiudz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/givctvphm.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gzkczyqde.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gqqfqrfeg.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gkbjfhzzj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/goaqrsoje.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gasgssalv.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gjleyrcpi.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gyfilkcbe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/getcninnj.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gnhlhtfct.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gofyhqmie.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gjbdsabro.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gboxlibix.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gribiipxv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gazjmovba.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmttavlyn.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyesmouqu.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gmgagtcez.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/glzszbryj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gaqtswpzu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gadtttaqy.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gvawvigao.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gnkxclile.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gzglnubuk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/grvuesdpe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/ggkofknme.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gncitvvqc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gdstkvmih.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/grzkyzosx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gajyauxnz.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/guwyvwmde.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gtpkzzbhv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfvlvbvds.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gixvfosjg.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gjrxbatke.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gfqrrzfio.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gfmbyjlws.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gkevdmwty.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gfwybrhjp.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gdtpijtiu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gamaxwbyt.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gjtglfpdi.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gaqjywgeq.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gzpfcwayc.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gukidoitd.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gzadsdoya.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtpegydsc.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/glnghuclv.sHtML


<!-- 参考信息 -->