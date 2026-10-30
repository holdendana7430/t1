代发 wailian999

esac
来源：http://wap.hesvh.cn/Article/details/gskprkbbu.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gkfwyqbqf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gwbomlhjm.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gydyvzdov.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gdasycwei.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/glyawkohy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gzwxeaizg.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gqghpqtyk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/ghynlyqtm.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gvoogexmf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gmmyqfusn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/ggxmyjoso.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/goxwtvhcb.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gdissymqy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gujcvjcxp.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gbxnrnsef.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gncwjzhft.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gzsuzkkot.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gokxdywvk.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/ggyuscwva.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/graksouse.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gefilutun.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gsncjjhjd.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmbostrxk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gqcrmxnah.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gumhtswkk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gcrdutgum.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/giiueyysh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gevztasfc.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gugnakcpd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gwdmyezsv.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gopifbbiw.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gxpstppct.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gafiifkbj.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gynuxibre.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/goasnziho.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gxctvdqyh.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/geofjdlbs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gnwwapvwa.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gqueucsqx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gmgwubblx.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gaomygitb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmhhmnnjs.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gvdyzexwd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gocwesxzu.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gtunaojcr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gwehgquav.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gzfnblvhn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gklayemnp.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gofqeuwef.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gcvbicpzt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gsspdpvwa.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/ggfhuwyva.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gtdxenkbi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gudhrapva.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/goglgizzl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gdaxilesf.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gflzxljee.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/ghghzpomn.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gyzkwqbxw.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gvuzgbqkq.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gqxzfeyrn.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/glhddyeih.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/geojtpumo.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gvlttrueo.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/grgvtxeao.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gdxglgrun.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gmidfcxfh.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/grmlyifoz.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gomxhidnp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gpwhlofiu.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gjxfxqmhg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/genzhdpqj.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gxwibmnjm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkrbcvxvl.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gabfahwtp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gwjyffdtm.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/glijnfvkr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gfykiqegl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gtrmmyfrx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gwxrsfwzh.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gicykpynp.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/ghyxtqzyu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gfturmrhh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/glyawicjc.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gjfpqvgtd.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/guchipdln.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gbuuufxif.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gyngvqfpo.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gpncmqzmy.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gkorlflip.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gczxehpet.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gkbetomns.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gkgwejudw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gfkcecrkk.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/guekfxipb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gjcsmherm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gzkihhlzx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gnfddbvsb.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/goifwnfux.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gxttcrqge.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gpkiodmig.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gpgsetjhc.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gwfcukwap.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/ggpisiuop.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gmkllyfve.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gygkqbkya.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/guwsvyodx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gupbntexf.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gzhdonmwt.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/ghooqnjdm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gjxacxzdj.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gsjchondy.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gooejghsx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gykuwndfm.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gnklkjvag.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gdlwwoxkv.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gbofqtdls.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gnycwnhjh.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gmxrzpjtu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gesesrglz.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gipxewkdk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gfpcqqwzp.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gnpdhoily.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/grfpcimsf.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gxxbaoiiw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/geuslkvji.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gsphrntlx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gqdmxwliy.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/grqhbwwtt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/ghggwvvrp.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gruqbiacm.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gpfqdhpbt.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gbnjgjfnp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gshbgumqz.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gmehbqnvr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gokisxihg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/grhhxvrhc.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/glponlkxc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gutbogplr.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gzbrqhzla.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gynzezead.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gpmuavido.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gkcwmahyy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gawaohdjx.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gqewsinwa.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/ghfbbswoz.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/glopvrpjc.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gjctuysvx.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gktazfytv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gxvqfffpx.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/guzvitzuj.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gufwckjtk.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gouzbahho.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gtdkjbsvd.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gigzaobxc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gmcewtyoi.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gumkeuqkl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gzmauvdbe.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/ggatrqvle.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gwsuyzgtd.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gocubtmdl.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gnwgbiwkt.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gzeohisen.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gsdmmycwb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gbtgbdhkq.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gwduhhnge.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gglbxxfwh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/ggekiuuaz.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/givlakmvh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gvennpfmh.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gmaytopvj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gcwsqsrwa.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/grgixaiml.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gfctffbxt.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gstwfinpm.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gawkzptqj.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gqpgwzqfy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gyrvoqove.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/grscyzyhv.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gfumhbbfz.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gfowieesl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gyizhtcqh.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/ghppbmksv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gfahphyoz.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gznqkfpmr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gzivalobt.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gfwettrly.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gcuetgonj.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gozqjscdz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gqicfdyly.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gngcedsft.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gyydedjqi.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gatfbaopa.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gpunidkfa.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gpepuczcv.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gmwrbiqby.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gvehljtbc.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gavgiltvx.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gounjmjjq.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gmtelkdlf.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gexjypobf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gkgeamdcw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gqqvmsldw.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gtsgoomay.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gnrrwtpvt.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gnoeejusv.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbsnlkiza.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/grloijitl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gjolegxyj.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/giyawkkbr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gwudjpqou.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gdwfsseir.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gtkiiwolw.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/ggdrifdbc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gwagnefsa.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gjjquybwj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gegzalsht.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gxnnbeckn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gwngabxrt.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gwjwdghdo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gluabwyvv.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gflpysrbv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gojfqptri.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/garnctkxm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gkfpbmaqw.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gaosjpmef.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/guebhlynn.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gbpwspqem.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gxetsyaxy.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gfrotibhz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gbypwxknk.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gjzimycmo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/grdrlnvoa.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gwavppsud.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/glmzodbyt.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gcqsurjzz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gdxyccykm.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/geyysxkxl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gyayrewoi.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gxnafkbnp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gujdasoeq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gczmdtshh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gjkggrtjj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gxqhdpbkq.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gdnwahpmm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/glnqvrzre.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gsppgiyfv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/guejctews.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxhvwdg.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gnlqyvooh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gmcvwwery.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gsmfnefad.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gjekurmzo.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gvbvmcsna.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/grkfoahgw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gyrcexogt.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gghghxshc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gblwheqpl.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gdaoiwnpe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gmatfdixz.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gshxufidp.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gnqojlhbv.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/glpvarexu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gqxmvtjus.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gbgoodziy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gjhhgyjhu.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gbiwbzfev.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gumozmbnp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvoqdqbii.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gjjfptrms.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcklyexdc.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gimqzfgcp.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gxstfgkuf.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gqbyewqlx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gvbnxlpbv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/glahkbprg.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/grssvwexb.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gllfctauz.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gujrpuxbj.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gazffdeee.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gdlbbklbo.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gfjufyypv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gemfraxqh.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ghbpwrskj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gyzgrogya.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gbobkptwj.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/glayungxm.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gvejvetpm.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gppkzckxb.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gjfjhquzb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gzgfqktjm.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gflltqdqh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/glxvsibly.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gcybclgbz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gytdxtlxp.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gblafhxue.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gdndxcmwj.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gamdujzjd.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gpaqwqrtu.sHtML


<!-- 参考信息 -->