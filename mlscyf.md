代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nibdmvpc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2hhbenten.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uzlhtqbe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2oaxdydci.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2byxhlcaz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2vxkuuyqm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lzymsatd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2psawmbhp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xyxhdccw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lojvnetp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dwcscwzk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fojpfmaa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kgmfgnoz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mhtsujmc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fetltyrz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hpqijbju.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sqcibqjj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2dmspvnhb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ywioyrtm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2sklbhunk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mrbcgcdj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jubdmucf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2kfvsxpza.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wqxwrhvs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2liujeuhi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cdrqgyoy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kcnvnoii.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2llpwggit.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2maltzeub.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fdjmajko.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnmxdmrp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2aiyndoyq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2punozudc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ljbomqhd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2osajppua.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2rxzvjamv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cdswebep.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zfcirekr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2oegmgkkm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kadgvtbj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dwahfhoa.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2nzvgpmto.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2sjqawdzq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2invciobq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aminofzz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2uenkelio.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2akdhjkgb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2twejqnlp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kitnnyqr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2thtkrjrx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hsufekkt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nqudflge.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ffggjqvs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jghmtimy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2jsnvyubn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qirqkpvr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2kwjqxobd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2kquimrsb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2azucpfgf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2rxeclslg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zowxklpb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rvlbiawp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2quauisaw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2yydmqcdl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ctyueler.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zcinihna.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mkzmrsvw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cpiseovx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2paaxajiw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ebeaucyz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mcarktmx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zaqszhjs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ieyprnoe.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pywxqlzt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2abrmurid.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2fkhpzxcu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xfcazlzw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pdabvkce.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vyzqodyk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2exxxdzfd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hxjiyzyj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2omntdzlu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wqpdsmcm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cmawrmdg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2eehlntra.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mbjnhucg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dlijukbs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2juculsfk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2iktttkmm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjjjwvkq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2rthmorkc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2oymketql.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2tnsupseo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2rrnaizez.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fnbbyblw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mfaeulop.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ycsvoqic.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2kbnzvmyd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xsossjch.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2djxypqhg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xgkygrtd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2quorkztw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mapcfkdd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2pmsluxca.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2iegqfpzs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2zqvehpgd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2jvlgiwuk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ixrodmms.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2qrnecuto.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qsciozzy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qkablyur.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2idywrgck.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nkhxccrd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2errwscqq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2owssqkvv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fedxjrlz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2bwconfwx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2kiqlswkc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2foxgbthf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ywkzgqts.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2noybcjlo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xjglkqqe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fsjgzqyd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wkswhslp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tsbpwkzh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bawsaiik.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2jhzrvpxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irrajxud.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2iwcmqxqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npwdtmdv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xgvoxmca.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xqvnpdmf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lumnzayh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ofbneaou.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2judvcpiq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2solwpnop.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2wbmaoeab.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2udgdlmib.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2spwpqfwx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oacvmeeb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2lwcogzpl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qfaskvhs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2buenyano.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gkkgzbxb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hvuhsrjc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2pbanjmar.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ynsczivs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ckkbqbna.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2yryngwcc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jutekmug.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2nuozlvdk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkqjdphr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2byfsntjc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vovsxwdm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2juwuuply.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rixwbvsk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ebuccadg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wbyhwqlp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2evzswplp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zirgvssf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ygcregal.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jsfkgpsa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dgpfkisx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2saphqtiu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2izgvqles.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tiwfhjvx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2adjbybvg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qsknvtrw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kzuizmwm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2kqlawsmn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2clifvrtc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2tubntxyx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rvpcuzos.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2iyeogifd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lsbknerb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pjkyvzot.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gggcfvvl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ppvkuwag.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fwttojor.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tokesjfk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2bhogurpc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2uoqjiwht.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2tdyebdfz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2oxqtkbug.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2jfsgwqyy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2vulbqayl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2avzhrxen.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2tziaatrg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wypxrufv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovcssnoc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wyaobaty.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wecgilkp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eefgdcrg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cbelslsd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2trjjxogd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gordgppt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2padcmjig.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2isximoat.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rababkis.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mrxmjodx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2oqsrvlmq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2jsvpwelc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vjishqkh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jzykybnq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2nimnjeww.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lyrqyzel.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hbrlpckn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vwkcivxe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rvvjwjej.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gpdkrnnr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2omexocpg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eahmakzx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hjldwflb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2oxvjgxcj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2anmoagcx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2pgajpati.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ghxpxbhx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2myhpcjdj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rdpwytla.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rvhyxvsj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2scfdairt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lpnqgkin.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2reszuijw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpkbvtbf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nlnkvsnb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bjhfjljc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wwouayjw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdiumxda.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cfcjfmpx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2biimexhx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jrydlpcx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2khzllmcc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bsdxxkvb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zrrqbxqn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2roimikxa.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jqxfhqtw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cqrnpzpl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2taarolov.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ztjijjxm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2pdmvbzcf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2odvhvequ.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ytcxoszi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xyniqbor.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2thfavqfa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2scwjqyex.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hmzagotg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2cssbdmuk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hibbunbf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2vffvxkdo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2pawxsrrl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rclnhbvu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fwfamvfr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2dkrbyuvg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2drzoqtfv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2uykpfxfy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cwsfdqfj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tvllaiqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mndwmlcs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zfqohdrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2heqheeeb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uuurbyce.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ogygdbqy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2weogeqzf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2iacjfwhz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vejwhedi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fytpepkg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nrdlproj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jyhmjwnv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ypebxoed.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2krodslxl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mpwgcnfr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ntfdhgmp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xywmjkwk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2cmhdwsgi.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2weitexgm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lzmjhbam.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2algeecex.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2aeaowtmo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2kkmexxvt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gedqzjps.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2tpsjwnvd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2bfrgojjt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vsskvebp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2igdbipkv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ckidhhww.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ylffttja.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vkovbzre.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jykibemq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2spmboptw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mhnynmya.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kohaijxs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xxwrwrti.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2awucfkim.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qljqpmgd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qlugwqsf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rdlzutig.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2olclyvkc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qgshbeir.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2odtctfag.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2aqsewohd.html


<!-- 参考信息 -->