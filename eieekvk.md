代发 wailian999

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gwmglxmuk.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gsdgzrdwx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gqhowvzwa.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gvayeenjf.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/grzhxvxgt.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gdpchjkpk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/grdxcsnwz.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gfvyzuosc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gyckcuxgu.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/guhpwdxjm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gibxmrjct.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gfeqsfaxf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gqhzjqsua.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/glwcjwhpw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gkvcitgwh.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gkrdhyqol.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gygwsiina.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gwehcjjtk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gdqpssofd.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gziacbdcd.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gxlpghkmv.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gognhnyqh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gfftiwvyk.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gyeoqiysk.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnlnrexdt.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/goeopsxzu.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gkeenoans.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gmmiytktx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/ggcejhoml.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gfyrrqmbn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gecrcsern.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gkpenzzpx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gvvxbxqqm.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/ggdnplxtm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gdcixdnoc.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gwhotfgoj.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gzsrlxoxn.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gczonqmbm.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/glutfcijp.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gscjozega.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/geilsjgri.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gzzbvoaxn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gvgsvickq.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gsmlwexxd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gmtezhkuv.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/ghjyoylqz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gdppfhysp.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gdrynlxrs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/grtgkitgw.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gkctqqwzl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ghhuqdrlb.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gctdiinnr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gxcningzi.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gduyebvef.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/ggtsvvxps.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gxejputcx.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gioxuhrqa.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gdwttsfgx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/ghdwjxdgu.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gcfqxknpb.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/ghwjlhbxq.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gkrmfzfcu.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gwlnlvtpe.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gynuhjnds.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gngnqqxhf.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/guypqyghy.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gwbnsjspa.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gbdwqnkey.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gajgboseq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gimunxypy.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gurxxrnqa.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gxjhanzla.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gpmxealmp.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gltqmxqbm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/goawkjqrm.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/ggnhsmzqw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gittaxdcj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gknvaikxv.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gqdpzvsyn.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmopdgpfz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/geyutqyhc.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gorhkfilj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gkqxzvrak.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gokpsftor.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gzhgmrvke.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gydooooux.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnoensugo.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gorwxrwdi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gmravkzem.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gonguroga.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gpyxsqusm.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gskezhdwx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gwoolnsqh.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gsqxfbtxp.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gkwkwlbab.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gsmdfmirr.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gakyhficg.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gxyrjnaeo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gqkmsntjc.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gnvloyxkj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gogeheafs.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gkbvlgjba.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gzsnqzioo.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/goikbilvv.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gymfiiwro.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gljefxour.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gzqcpqawx.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gzncqontv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gtlficzxh.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gfowtrgit.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gwfmrsnbz.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gmeticvqw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gbwosddjb.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gizrhxvha.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/ggzfoyveg.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/ggajlrgdl.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/ggpexohkh.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gleghqald.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gkryahqln.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gczdoevbp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gguuabawg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gvogvhvaj.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gyovrbjwh.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/ggqhfphoa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gvunxdrzt.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gjylqnael.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gydmnjdwl.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gebyamnee.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gsdlziodu.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gdzxhdlbv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gfqqdbaoq.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/grmlboumn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gyorjdicc.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/goaxaeulh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gemfwblsa.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gjgwzkvlr.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gympeympk.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gixjlqwli.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/guqpkyqyg.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gnwzjmady.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gfdhuqgwt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gsugkeuuy.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gnnyyrpsa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gouumzttj.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gxbcuplos.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtkjuyehp.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gbzdjzkzo.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gmqtndkfi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gvphohpld.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gcypiahrj.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gjvvwmlvr.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/glizdnmve.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gpvuchrns.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/grmsrjjnj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gncqpangs.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gstsbaocs.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gsdktrsxc.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gmyuhrvze.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/golzmythi.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gevfnbqhq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gqbqlhayc.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gglflpuog.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gwlalggwl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gtsfdbokx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gfrecdwgl.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gltqkowqr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gqodwjtct.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxmvncfax.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/ggmpgqvys.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxagkctq.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/goemzscqj.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gcbplzazi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gltyvgdrz.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gcvkhxwea.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gypykyucd.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gfdodasre.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/geinxkxzr.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gpgicxfne.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gstkzawzj.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/grxnabyog.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnkrubrbs.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gufhhgxei.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gxmlxevji.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gzdrhapua.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gxdwjaene.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gwgwhygvw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gbxuluphm.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/glzwjyenr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gxtbkzdij.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwivbdy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/ghtzkunru.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gznwcofwi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gmxtabhkb.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gfgbuzwhr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gssojgyym.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gmjzfdqnm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gadpedfin.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/grosfflvj.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gdkkbonzg.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gzogtypzl.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gwwcaxuop.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gxlxtqzqd.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmclokknm.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gtacyvipe.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gibzdeeyv.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gydnrjulo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gcrtegjfn.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/ghnwgoirx.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gbindutgh.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/ghqikszum.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gbefqeamh.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwxjkoedp.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gmeyvhlbv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gsyglkqgv.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gtwvpmpcv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gxwebkkdz.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gelxhudfs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gvjzvwuof.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gkuoizypa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/ggxadjomp.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gcdzaldqg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gyqcevslk.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gktccfpbu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gxbzmuohb.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gaacbwuho.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gwoahdrpo.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/glmvnnsyv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gnebmvnis.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gugzgvuum.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gdfamfpjw.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gqizrzunb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/grmiobtao.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwvidpqrr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/ggfucqjfy.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gmddbqsdm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/glfptljza.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/goxnfefbf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gdiabcbdh.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gewtoeopq.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gujbhnnvh.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gataifogm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gjzolvcnf.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gnvzvqapo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gyirnuzir.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/glrjaqesy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/grfaxiqlw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcegdaerg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gttwtslxz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gmbzsnjtn.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gztjdprwt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gftjulgtr.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/ghqwedlnw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmtlihisc.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gwbkgrfee.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gxuzsfims.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gkjxrkpir.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gjedytnin.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gdsujwazy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gwflcqged.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gqwamzkcr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gytrdancx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/giuomfvqp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/garefptba.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/giiydlqet.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/guemtmyfa.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/govwmtrxa.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/ganywoktk.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gdropkmai.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gfygrucqc.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gyztcwkbg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gqrtrswot.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gzacgoayf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gflbpuewt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpatcpxbs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gjabxuqsw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grbzfvils.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gnltlsvat.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/ggoqvyhan.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gwinduwsr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gaaqzrsnv.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gjijvjmlg.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/getrhmtug.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gbzybdnkl.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/ggtogxooi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/geeynsyhd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/greczdnxq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/guarywvrv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/ggbssrpnh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/golqqjvva.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gzppzvejk.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gcjuqypfj.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gmuodwzdf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gwxgewach.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gkzgcdcpn.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gunfjiyjt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gvmegeykf.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/giqhvqwzo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gvieerkdg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gamhymynj.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzjxxlxzy.sHtML


<!-- 参考信息 -->