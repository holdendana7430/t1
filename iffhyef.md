代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsazkfzwv.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/geyqymxuh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfeqmdwp.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnlhkoeny.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxbyzxnyg.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbebfonay.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/giyczautq.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gghbcidit.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqquvepr.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gyxxsnfxd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxoirrxos.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/glvduztuz.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmxpypgji.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtocytxsf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcabobqpt.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gzgxfacbq.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gavyxauxb.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/grnrlohmy.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glssjaquu.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gurqndwff.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicrlgwib.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/giowbrrcu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmyxspgc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelviohjl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gveiredsq.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunkplizj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gunuoqccp.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/glayjcvxd.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwsnrldn.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gopmulvbp.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmpnyxxo.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggearklxk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/guurzrxun.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwpgglyb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gteabsaom.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaejhysc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcvxcemi.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gvulnugvs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmwbpygdp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gkqvofjls.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gdugieoxv.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwxeagom.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkjjlnhn.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gvnrxsras.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gamqnvvdk.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gatarlcpk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgexqqim.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grzxowxan.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grqkmekyi.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlqxcucp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkahaavjr.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/grkeifkfk.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/guyvhwdds.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gnbwvicmm.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gxbwxeneh.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gmppohjzh.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrqvzgen.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxjyulzd.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjcrzrmy.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcdgjbwsm.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gmsqhslse.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgjmejjj.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gohpvhctt.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gzglqbfoh.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyqddzes.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gzlwqhftl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gypgtfoua.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcvrhhht.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoixplnb.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gegitkpsp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasctbwsu.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxlewzlz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvmzyfdp.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/guxisngpi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfafytzuo.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsqnoxbw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gulsezsiz.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwxkyyeg.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcqsmmvfz.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gtlfaglia.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gzwrdkrsq.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/givzaonpm.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtfoeaqbo.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoonswzo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gzemptgct.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/grgmqssrk.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gooohzkui.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gvyoighxf.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/ggtqcmgzv.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrlongnr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnvrbwjh.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/guznibden.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaeztvyb.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/glulshhff.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gowbvrcyg.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gigoqjomn.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjvmdpug.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlejqzeu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzedceqh.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwgkmomn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdjmlhgy.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmxbqgfu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfehuiuaw.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjluqhhmf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gifyajixe.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzzisnud.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gdnbvcors.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gktogjlkc.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gvayubewv.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/glnopgrww.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphgkuvcj.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjtuahej.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gfzydwsma.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gfvcpdqah.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gwawwhzqf.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/goragyddm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzrsumoq.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gopgkongz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmuzflnr.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzlgzays.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gperwhivy.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/glzrlutye.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiurxtwq.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gateuotlr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gxfxgaupq.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gprcwlnzs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gjerbdqdh.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/guozklvdy.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghwxhlzn.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/ghvyvrdyu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbltrelqy.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gsxmhgiew.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyribqkj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gdxnutjte.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcjkkkpy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdwqmguv.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/galtrsskn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyzuatud.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gexmybdbm.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/goudazsac.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gijxgxdsu.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnulquesj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gygsdfsdf.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfmqqlnq.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gdkxmbvyz.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gfslspqme.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcvqpvaq.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gbwoiabbf.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqlbrgac.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunqmuyez.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiwwqpbd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gravvhojw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gscdajbzd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyjpicex.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/ginsstsbf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gvisrjkaj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gntfuxxcs.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gakmapccd.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gejxbzjnu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybtafalq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gylvrbdhd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gzwqiqpch.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gpstvdhjr.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gniqpyhpo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxjcwknx.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhzijfxr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmfruoat.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjajhzdv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gosjewowa.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gweawfnbg.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcngubhod.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gfulfvbzb.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gilufliod.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsupjfgj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gvjeyzdsk.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/geqvrxvsu.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/ggnzdcvub.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gfvwmejic.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/guourbedw.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gokqoeefi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlxpbnga.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gkcdxhnae.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gdvqwrbgx.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/glqleezho.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjspqgqda.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvaockek.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gzzgzkcqg.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnhjbsvl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbmelhtl.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhpwvame.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gmpokjdti.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gekidjnhb.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkggdhlw.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gosqycdcz.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahhmvvcf.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcutxymj.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozkikgsz.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxkykmqeg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnihuoci.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gbreglbye.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gtpmntjmj.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gdpvjnvph.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/giaxnxosb.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpujmxpfp.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gmltsrayi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcxrroqkj.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgqzjnfe.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gttjmpcin.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjyqpnii.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/guswfzgtv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaitzjtu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcxtconn.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/geimmeyoy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gebpqgask.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfobmwvl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/glvtmejzu.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gvdbhkcfg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gyupiyjxw.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/grhhtnakx.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/glpmvchlk.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gscczivle.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/giqvladgg.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqgqvtyh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gettirxrb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdiflhwe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmtlzbuc.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjytisobp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/guryhcwfc.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/glnljriib.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrafzseu.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkkiawij.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpltjbgpg.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gehiytovz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gdkdizynl.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gdwqllszn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfacvpyle.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grhhpzwbf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvhwtdcz.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggxvpjfch.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gumczpzha.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnstmcgd.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeccfdit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gefepgrwy.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gckectmno.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gooavagyt.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghukrjsuk.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzakhyft.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gnoasgyxg.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwjrgvebs.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjelxbmfc.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghftjbceo.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/grouxclsh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gtjmywafs.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmzdmqyp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnggjayib.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvvtlhxy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcocrpzig.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwynkitf.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqqmedah.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggteudvcc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrekxxdn.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gwbdohcgi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/giviygpqs.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjepujajb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/ghflgzymj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggghictjl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevdcfwkb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjlaiutdb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwhdisik.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gglyxkosy.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/goqdzwgbf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfnpdgmg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjlzuguq.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/grxsafypj.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/guhjcbywr.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotjyepxk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjeoueez.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjysfvpfl.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/goditcekp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyhfkqwd.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyfzegsc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpcqdacj.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gcjmeztnw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grznzjrrr.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjzwhkbf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfinliffv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gkszaxmqe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gazsbgdze.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gzhkparrj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjqzhhha.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggvxbthh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxucdqdwc.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gtzlxgftn.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvcfhyzqn.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gcyvqvfdu.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonfnwkfu.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/goyqnpvtg.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbqhzozb.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/goanuosxq.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggwumdkiu.sHtML


<!-- 参考信息 -->