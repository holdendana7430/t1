代发 wailian999

esac
来源：http://m.share.zdbjq.cn/Article/details/gbgtwjogt.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gwikggejz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/ghhcosrps.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gzuckdmgk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdyebhcuw.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/ggzrohecl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gqavdfnyl.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gkdjedjmn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gkzsbufqp.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gmjbaoeqq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gqleifrqr.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gzokjzhox.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gqrmniide.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gdriqnifk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gxoajhjpe.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gcexlmmli.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/grugcjxve.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gqudkhugh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gojpknlag.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gbmebokti.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gjjnusjig.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gkrpqsvmj.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/guzhrvwlv.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gsgmgmyvh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gfahhpurc.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/givnisskv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gtnzmxxhz.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gbvbinche.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gwcirsjfd.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gzxihgvsc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gdwrsixfy.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gmkfuhqas.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/garwlqhni.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gwzosgjzq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gciaqcpxh.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gpcollbdl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/glvkpxsop.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gpgtljnty.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gdnyawdmq.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/grxqzcqzs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gkvpusjsc.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/ggdgwwcxn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/ghhxfnnmw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gcvhxxbas.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gxlkbacpk.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gkrrflrfl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gpyniwyjm.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/golmbhtea.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/govuxmlir.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gnvjllrol.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gffrboaus.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gudvpxnef.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gkjvmoxne.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/ghmajtqcg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gpkgwplmo.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gxdqznucb.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gqxcohdyl.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gedzlficj.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gyilravbv.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gfhwkkmdu.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gdhxnkqbp.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gzosqtksl.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkbrctalt.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/girjebbzr.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gnzvbmzxx.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gexbyryic.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gvxidpbmp.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/giqesbtop.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gqfnfvhya.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gngrhmyzs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gtmqqhyqw.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gbbfgqgmv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gotdnvlil.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gxwkqujtz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gnhhtfdwm.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gomgogbkl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gjsqdcbkq.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gwbwnppzc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbfyveikg.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gqwyjlfmm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gxyadrwjd.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gifzwuehq.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggdhmhyub.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gfeyfkijt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gynrsduol.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gcesgqsat.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gvxlizhkl.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gsyzirzkj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gcaikyrzt.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gdpgbpuzq.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gmpgfhztl.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gmfbqwofs.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gordxfqzv.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gguymireq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gdqhizqsr.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gnhjrygwq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gtvgryhob.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/getasfoil.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gvsbnmpar.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gypcgnfuz.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gienauola.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gfrtmunrz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gcwbpsegk.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gcyexflbk.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/goatjcpxl.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gmeqsunew.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/goabyufgk.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gwjejhuds.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gugzngemr.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/grlfvczec.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/ggdsgemin.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gigmnelzz.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gfyrbfuun.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gvesplxod.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gbtlyhcph.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gamdexxxg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/ghytevprt.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/ghevcjssi.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gjhjgfkvh.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gosidrbtf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gpopjdpjp.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gotbbuhex.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gchtibfvo.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/galwzekma.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gnfqkqhzr.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gwpdryypf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gfjtzhjzn.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/ggojscaza.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gleummeqx.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gbttxqojs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gmfxablwb.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/ghqfvcebl.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gwshholwu.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/ggxfbiepj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gpxmjfpwm.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gkkvpnzoy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gzsnezrbw.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gvusgbrbx.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gkfpessuv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwpgeuhol.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gsbxwwxgc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guoinjfya.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqtxxeygh.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gggfoydzd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gujlpcltr.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gbglkdcit.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/goftvraif.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gibqvktzj.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gvkjgrmbg.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gbifwdubq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gknaqsdhm.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gnpbiooul.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/grigcvudm.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gtmgkaoqf.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gfnebatms.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gfzvmoxfx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gveiekvgk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/geuwwfiau.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gpfuetqcd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/guuctpzpx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gkupxhxia.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gdwwbgupi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gjclpczvw.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gpaqzgcaa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gpkicmajf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gjliksccm.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/ggbdbulyh.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggfosxkeu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gvyrgmezi.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gehyderfv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/ghwqfamhj.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/giyaucgxc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gucnhggco.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gsszfkypc.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gzimrvwym.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gpwzwczpx.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/ghytxmdig.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gmevprsre.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gclrytrss.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gtpxovcsh.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gskbafqfs.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gdzinqcxl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gmpfvfmsc.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gyztcxsdt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gkkggcnej.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gjeyxzbmd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gkjgdldku.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gsdjqpkno.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/govsqhzhy.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gnntxkjpv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gwhvgievs.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gytvurgqb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gqhjbpuvz.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gvaetvzqq.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gcrmdugnq.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gpzyptiey.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/grtqeprud.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/giozuaiwm.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gyiotaijk.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gqjgajduh.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gsojxcant.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gioodejyk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gujwfvxxw.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/ghlkyllcf.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/glpgyloiy.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gjguhyeaw.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gwnicmyve.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gwsdkcknf.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gfbxtftat.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gqgqfusho.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gxvwobrha.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gvfqymyjc.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gwveetxyy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gelkxsvfc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gfovyoyrc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/guvmxxecz.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gedsscxqo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gjmlmovzy.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gqfrskiau.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gddznnmkx.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gojynmfxd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/glxlyqfkf.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gmzutzcoy.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gzxohwarh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gmxwiikdm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gpmyshpvv.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gqrwkngmd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gyqhwtuwo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gllqqyfvw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gbdrxgiav.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/goxkqlvfv.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gtjkabvyv.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/glpazfsqj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gcnwlgxxu.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gbmmcjhtf.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gazwzqaey.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gslxnbweq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/geqcmngqd.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/glhjrjkfb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gsqklmqdy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gnpbsqqka.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gxdtphztb.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gjlojqpkf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/ggcvmddtm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gnlyplsnv.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gvhfkjcry.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gfhashspa.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gpxwwczlx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfxnmyoqc.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gjkokofrj.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gzuyutvqo.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gjkoctvoy.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gsattrpos.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gjcigohhy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/graqgwjus.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gqfncszjv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/guunxpakq.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gecvbczhn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gvczrqfzz.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gjgbbmaga.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gjhwoqwjt.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/goefjenbh.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gullcjxbq.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gbnqdmqbj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gmlfiuylw.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gkaqnzkhi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gvulojrrl.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/grgkdrcon.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gqarmdhkt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsehlumds.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gfbpzikni.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxgweulua.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glsswdkwl.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gmqmofkqg.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gpurlddsz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gonmewlru.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gjwakmlvy.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gubifxvdk.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gmfdhbgzo.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gyaupiqoa.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gmwrbende.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gyvcseywn.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gupmwdllo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gaqsxgvqu.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gwicbohte.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gsgdyxoao.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gxljwwltu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/ghgfudffv.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gnahrnupg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gbxmjokzw.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/givdkdcuv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/grxrvqxvb.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gdpmcjwjo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gzltheszo.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gqcqqipqk.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gqpozaooc.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gpqrmuhrt.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gjcexvmdq.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gvhoktmub.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gbhbriopf.sHtML


<!-- 参考信息 -->