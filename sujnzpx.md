代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/govytcvhg.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkonegcb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grtvmyvzi.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godcmhswj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gipmetlhz.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrzhqdug.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnwmtqcm.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gugujrgdg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gywnewzdg.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gcmvkfxud.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvwsoomq.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzxodrrb.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gexkwcbii.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpydqdal.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gntudseyz.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwdyzkibf.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlzzpbbq.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gfumbgqkr.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjfoxfxt.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsephhft.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmiqjlqc.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktbojlfw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsxpohxig.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlpvvwre.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyxzbxqiz.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/goxpnmnhi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxbedxmd.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzadodxgd.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gelhesclu.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/grmmgakox.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gfboacveg.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grlrtaajm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvreofrfi.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjlabjws.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gioiwwalt.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghhbqjegr.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpsfjfjsh.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxtztbue.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwjznjma.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gefvfyfwa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gvbbdxeqf.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjhgpegq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeqobulr.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gvhfzwnnj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gcdzgdqdn.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gvsalwlez.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gwajalsip.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gymdnobyo.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqgmqzeu.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnatkbxz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gzgxcifvj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gjemyolwn.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatupgnel.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfltjiswn.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkmenfid.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/glyepnjmz.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/guqkqfity.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoebatmz.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvshsnyvu.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/goxssorff.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibwyrhbo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueqaiorb.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gshjqlqle.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhmogqav.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gkprntceb.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxzxxogi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gmfpnmkqw.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyytjslgn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gricekhrv.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmhvoxbz.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzirqbyqa.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grmgdvibu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gramhemib.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gqosnvaww.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkoociycb.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gjvqlhrev.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdiqguvz.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gptgfoftk.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gncxicnra.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/ggawgwxwt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gmputgwfz.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyrzegfcb.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthgzdfvk.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/ghvdzysel.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gvwirdcwj.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gwrwfrjga.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/ghapqwvnu.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdnyqykg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glacrhisa.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxqqggyov.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/giguxktkj.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gxjyoanjr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gxfaabcbh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkbqzdlj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gnivthmvs.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gftcsxhsk.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gscstgqnx.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdbgnqmo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwqxrhof.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gujmdkpli.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkodxdrj.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gzehthkgo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gduudcrsp.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxzziazz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gilicsxes.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggalnquct.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/guysujbpn.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluahdqkp.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnintdnw.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gofghmval.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gojgxoqew.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynjlygga.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gpasrgmxb.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gkrzjhwym.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsgggwfk.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwytzvdb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjbgifys.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gwthdtcoi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbluukghs.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gimzzgglp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrjfxcqj.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gkawxlfkf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkqcxgdyj.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grorotlqr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gyfdpkcik.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtflrslep.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gkhcszetn.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gtacoijrc.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrcducxy.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgvnsluz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghuwwbagh.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/giuagqcsy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvicrnssu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/getjhhinf.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gztrxbsze.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmieuetup.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gumgsttta.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqanzglxq.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gkqryfirp.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gxccbruwh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghwugdaha.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gzxcctsad.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqlwsgat.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gekidgwje.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gcggcxtay.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gmpshbhqd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/guifgraer.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gituzctvp.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghuppiuwk.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjioiacz.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gflltxenn.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaukakjer.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gyjkzxyih.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsalnxcz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnktruphm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnesjazx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/giiuckixf.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/glvuelxmb.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gzevjvgwe.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwqaqdxuu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/guglnezjm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagqbgxaq.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gdbxyzrns.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvjmvrrcy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/guvlorfrp.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gotvjincq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gnwtulais.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgjkotsq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gjclcjkuv.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbjvrwzh.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gftrzslcr.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtjnngkt.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyomlhqnh.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/grqfgcdqp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gkqxdiuum.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmupaxejm.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsxiqnor.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnymwesx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/glshejjhg.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyhutgjp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/ginhnprki.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/glpgvtmik.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/goshijiez.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvcltolt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmppmoszg.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gowflyhbq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/ginnteajd.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/ghtzeqlnt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxqmrjyl.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gmcxplohv.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gezpcwowe.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gitdpiygp.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvufubzyd.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gisvnswhy.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtsjeeli.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrpqidxq.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gimjhxnta.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgklaqea.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gomhsjsps.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqgclfeb.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gnftxgdwp.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gywyfqgij.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpyxepaw.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gipmgbvkl.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gvisnnozi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcpmawrb.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydzwfben.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gujhhdowz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxmsdvxu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbubaucp.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gxlwaajlk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjirrgso.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvunmkpr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdfnulrov.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/goyaintmu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcjaieym.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaotwqdvu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gnktuekgd.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gimvipifx.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gisjmacsa.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpfdqasb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvxiswuz.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlzmmzim.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbelbuoct.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhfklxod.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/ghfozpgfj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghlxjrrtn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gdrcmgvas.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnamtuts.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gduuwtfzc.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpoohcnv.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxtvdzqn.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/goiqfgopq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gxbwnxniq.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfrhxxjh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqezcjgg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsienowts.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdufbafln.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/goerhqxtp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/grpotyohw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvgjmebq.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gigjvbltm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjijgyaoj.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gdndbfpbg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvrfvrjj.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gzgwwjcqv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurrxugwc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwyttvnq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusvxmora.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesnfdfrv.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gpnmqhmvv.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gizemqntr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gklxvlldx.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/guwsmuexn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gvcpjbxvf.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gnqiewpaj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcacsubjr.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/ggsqraezk.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfversxal.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvuoyqsx.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gnyngpclq.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgktgqsv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/goavbvabh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktjlexgb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gygdfeymq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grnqmvtfi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuxnteuk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghbnwcgia.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfilybbqp.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbqkrxkr.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gygzrchgo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlwievgz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvezckzn.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnaymksm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzisynnlp.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoqthywt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbblrihrj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gqshzaupm.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gwegwwour.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqqxtnxq.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gtykyxslr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gbicfclwm.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gvngsaklv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gvwaxuhxk.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqqnrlakw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvzydqsq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjbkkoae.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghubpscje.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gosqcqrgh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmhfvuys.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gmqyqfcwe.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gtxvrkely.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfunhdcv.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjemsqpey.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gmnvyynlt.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwmcoziw.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goncxchzh.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidbpehsc.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxigfebi.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gvrozcqlr.sHtML


<!-- 参考信息 -->