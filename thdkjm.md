代发 wailian999

R. Bash 专题
来源：http://hz.xylfe.cn/gtfuenhcix.html

================================================================================
来源：http://hz.cheryme.top/gtbtalvggz.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangkeji.top/gtceszocao.html

#!/usr/bin/env bash
来源：http://hz.ybcxt.top/gtojzdlrmm.html

set -euo pipefail
来源：http://hz.dianchejie.cn/gtdieadcsf.html

[R02] 变量赋值与使用
来源：http://hz.pengpengdd.cyou/gtltomfrep.html

name="Tom"; echo "$name"
来源：http://hz.wangshuangyany.cn/gtuorihbts.html

[R03] 只读变量
来源：http://hz.yuxming.cn/gturjsvbwg.html

readonly PI=3.14
来源：http://hz.jqgfzy.top/gtuylgjwlf.html

[R04] 位置参数
来源：http://hz.gotoacloud.top/gtuqtcbdin.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yvedp.cn/gtwfyrhaau.html

[R05] 参数默认值
来源：http://hz.shzxlz.cn/gtcnonrgsj.html

name="${1:-default}"
来源：http://hz.zhongyouzk.top/gtbvhwuhte.html

[R06] 判断命令是否存在
来源：http://hz.zycfv.cn/gtxbksazmg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhiwuduotai.top/gtnxxmfuzh.html

[R07] if 判断文件
来源：http://hz.ehwqpu.com/gtnfhpgiii.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.birdmap.top/gttdcycghe.html

[R08] 数值比较
来源：http://hz.316326.xyz/gtgzhpbyvk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenzaomai.com/gtwqryvgyi.html

[R09] 字符串比较
来源：http://hz.ydzc1.top/gtmltujvha.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zycfv.cn/gtcozvaxkd.html

[R10] 正则匹配
来源：http://hz.iojbl.cn/gtyjlfwary.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yvedp.cn/gtexnzuflz.html

[R11] case 多分支
来源：http://hz.mhx1999.top/gtbuecliqh.html

case "$1" in
来源：http://hz.xuetiantiany.cn/gtzuzlduej.html

start) echo "启动" ;;
来源：http://hz.redwolf501.top/gtmyefdzcs.html

stop)  echo "停止" ;;
来源：http://hz.ppjwa.cn/gtsmudupbj.html

*)     echo "未知命令" ;;
来源：http://hz.zhoulong.xyz/gtxsqqebzd.html

esac
来源：http://hz.0kj1m.cn/gtvanqhdza.html

[R12] for 遍历文件
来源：http://hz.gzhubu.top/gtlllrqhwn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gzhubu.top/gtlmjkekoe.html

[R13] for 计数循环
来源：http://hz.hysaishi.cn/gtmlbtaqvk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tanke756.top/gtgmprbznl.html

[R14] C 风格 for
来源：http://hz.yuanzhike.top/gthugesirg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shuidangran.top/gtwxfefiww.html

[R15] while 逐行读文件
来源：http://hz.havefunace.top/gtcnvqydvr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigufen.top/gtstbidcou.html

[R16] until 等待条件
来源：http://hz.shanyushiyangkeji.top/gttvsbuzjn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtwnddkrtz.html

[R17] 数组定义与取值
来源：http://hz.chenlongwang.top/gtkhlnbmmk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cqqwz.cn/gtizerbidc.html

[R18] 遍历数组
来源：http://hz.sweek.top/gtlleunjub.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhijiandao.cn/gtzpdqmfed.html

[R19] 数组长度
来源：http://hz.gotoacloud.top/gtyvskrktn.html

echo "${#arr[@]}"
来源：http://hz.jiagoushi.top/gtzsdxcwqw.html

[R20] 关联数组（字典）
来源：http://hz.kuanghao11.cn/gtoixbxnlm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.dashuyun.cn/gtrfccwmkb.html

[R21] 字符串长度
来源：http://hz.nwbrower.top/gttmqixyiw.html

echo "${#s}"
来源：http://hz.nwbrower.top/gtyxscelwv.html

[R22] 截取子串
来源：http://hz.hongshengwenyu.top/gtdpyssnuy.html

echo "${s:0:5}"
来源：http://hz.hywenlv.cn/gtsfjojauu.html

[R23] 字符串替换
来源：http://hz.sweek.top/gtgjktxilp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shzxlz.cn/gtxzsscinp.html

[R24] 大小写转换
来源：http://hz.zhengqikj.top/gtfomiewmm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hammf.cn/gtvkwnqamu.html

[R25] 去后缀 / 去前缀
来源：http://hz.tianlin.xyz/gtsihofzrg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gogol.net.cn/gtgjibcadz.html

[R26] 命令替换
来源：http://hz.zhijiandao.cn/gtwrrjnmft.html

now=$(date +%F); echo "$now"
来源：http://hz.gogol.net.cn/gtvcsqjbem.html

[R27] 算术展开
来源：http://hz.cucudq.cn/gtpjnqwcbn.html

echo $((1 + 2 * 3))
来源：http://hz.hysaishi.cn/gtqhopqeiv.html

[R28] 浮点运算
来源：http://hz.snrcjt.cn/gtftaxkhnu.html

echo "scale=2; 10/3" | bc
来源：http://hz.fzhhl.top/gtbcauylus.html

[R29] 定义函数
来源：http://hz.xylfe.cn/gtseosjnwe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gttcdynbxk.html

[R30] 函数返回状态码
来源：http://hz.fengsongda.top/gtznbgqhhs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuxming.cn/gtgheqesjk.html

[R31] 局部变量
来源：http://hz.nanxuanxn.top/gtiqzvgkqr.html

f() { local x=1; echo "$x"; }
来源：http://hz.xinyue.icu/gtxdwazffi.html

[R32] 参数个数校验
来源：http://hz.snrcjt.cn/gtmmydvupt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtxpnnqryp.html

[R33] 捕获错误并提示行号
来源：http://hz.jiagoushi.top/gtstperfby.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jiagoushi.top/gtiphrrxnb.html

[R34] 退出时清理
来源：http://hz.aibaodan.cn/gtqqkneklv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hongshengwenyu.top/gtlwgwvgcy.html

[R35] 后台执行并等待
来源：http://hz.cucudq.cn/gtgtgpaazj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnqzz.top/gtoqfapgsy.html

[R36] 并发执行多个任务
来源：http://hz.jiagoushi.top/gteecdxwzy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yvedp.cn/gtkcyfmkdk.html

[R37] 把输出赋给变量
来源：http://hz.quarkkingdee.top/gtiftjypja.html

files=$(ls -1)
来源：http://hz.ydjk.org.cn/gtmufaypva.html

[R38] 管道串联
来源：http://hz.tanke756.top/gtrbqcxnhd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sufxvd.cn/gttnifyayy.html

[R39] 重定向标准输出与错误
来源：http://hz.yuxming.cn/gtvydkwykp.html

cmd > out.log 2>&1
来源：http://hz.sxryk.cn/gtsweufjwu.html

[R40] 追加写日志
来源：http://hz.tanke756.top/gtcnypeggm.html

echo "log" >> out.log
来源：http://hz.dashuyun.cn/gtcwkwpiqn.html

[R41] 丢弃输出
来源：http://hz.sufxvd.cn/gtdsfxyewp.html

cmd >/dev/null 2>&1
来源：http://hz.zhijiandao.cn/gtgekfttxe.html

[R42] 输入重定向
来源：http://hz.hysaishi.cn/gtbomxsmnk.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gtdkdqyadq.html

[R43] 按名字查找文件
来源：http://hz.jinqigfzy.top/gtcvnnogjh.html

find . -name "*.log" -type f
来源：http://hz.shzxlz.cn/gtnlepfrqb.html

[R44] 按修改时间查找
来源：http://hz.sxryk.cn/gtocmaqzui.html

find . -mtime -7 -type f
来源：http://hz.c1oappe.top/gtpuitquog.html

[R45] 批量删除
来源：http://hz.sxryk.cn/gtksnsewej.html

find . -name "*.tmp" -delete
来源：http://hz.xinyue.icu/gtexguaska.html

[R46] 递归替换文件内容
来源：http://hz.shuidangran.top/gtirzojxuf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.kuanghao11.cn/gtuumyegte.html

[R47] sed 单行替换
来源：http://hz.smart0.xyz/gtswffggcr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.316326.xyz/gtudnnbyls.html

[R48] awk 取指定列
来源：http://hz.chenjidiqi.icu/gtammjjexf.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhongyouzk.top/gtnrofpipn.html

[R49] awk 带条件
来源：http://hz.yangfankeji.com/gtvyhwsnip.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xziqi.cn/gtgejgchai.html

[R50] awk 求和
来源：http://hz.xuetiantiany.cn/gtzgweqqwb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jianghu66.top/gtquphpllf.html

[R51] 排序去重取前几
来源：http://hz.zhixingplan.top/gttaknxecp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.quarkkingdee.top/gtckheayzt.html

[R52] 统计行数
来源：http://hz.gogol.net.cn/gtaiuzcjoe.html

wc -l a.txt
来源：http://hz.yonumen.top/gtswjnfdwe.html

[R53] 查看文件头与实时尾
来源：http://hz.9152youxi.cn/gtitrwifkd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhixingplan.top/gtoahtmttc.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangtech.top/gtbvlobfvb.html

diff a.txt b.txt
来源：http://hz.gogol.net.cn/gtcrutbklu.html

[R55] 压缩与解压
来源：http://hz.zhengqikj.top/gtraugrzko.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tian-w.cn/gtammjzcaf.html

[R56] 远程拷贝
来源：http://hz.hysaishi.cn/gtunzerinc.html

scp file user@host:/path/
来源：http://hz.pengpengdd.cyou/gtaheisjpy.html

[R57] 远程执行命令
来源：http://hz.yangfankeji.com/gtpzmchdie.html

ssh user@host 'uptime'
来源：http://hz.gogol.net.cn/gtontscrxc.html

[R58] 下载文件
来源：http://hz.mhx1999.top/gtmxqrbsrb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.snrcjt.cn/gtvaxrrqqp.html

[R59] 发 POST JSON
来源：http://hz.havefunace.top/gtjtwpofqm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydzc1.top/gtzwhfvdym.html

[R60] 只看 HTTP 状态码
来源：http://hz.snrcjt.cn/gtexcybggm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.bjfxy.top/gtvdkhijqw.html

[R61] 磁盘占用
来源：http://hz.gaohongyu789.top/gtaksqmmcr.html

df -h;  du -sh *
来源：http://hz.tian-w.cn/gtpfxvhakg.html

[R62] 找最占空间的文件
来源：http://hz.cashguo.top/gtzxiosdsf.html

du -ah . | sort -rh | head -10
来源：http://hz.316326.xyz/gtbrbytocm.html

[R63] 内存与进程
来源：http://hz.hnxiangtu.top/gteleuqhhu.html

free -h;  ps aux | grep nginx
来源：http://hz.mhx1999.top/gtesequgey.html

[R64] 结束进程
来源：http://hz.pycfn.com/gtveysrnbw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xziqi.cn/gtfofgwmdq.html

[R65] 查看端口占用
来源：http://hz.jinyuanbaomall.cn/gtookpexzd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gaohongyu789.top/gtprihddkr.html

[R66] 定时任务
来源：http://hz.jqgufenzy.top/gtdxchwjdr.html

crontab -e;  crontab -l
来源：http://hz.andypj.xyz/gtqvrjoozn.html

[R67] 生成随机十六进制串
来源：http://hz.gzhubu.top/gttilzleza.html

openssl rand -hex 16
来源：http://hz.yueranfly.top/gtmfvwfgyh.html

[R68] 计算文件校验值
来源：http://hz.smart0.xyz/gtuhoxyyju.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yongpay.top/gtvgkxdmny.html

[R69] 生成随机密码
来源：http://hz.zhengqikj.top/gtfhqcjojd.html

head -c 16 /dev/urandom | base64
来源：http://hz.mhx1999.top/gtlifccicn.html

[R70] 时间戳与互转
来源：http://hz.cashguo.top/gthwfbpriw.html

date +%s;  date -d @1700000000
来源：http://hz.sxryk.cn/gtlvmxveys.html

[R71] 日期格式化
来源：http://hz.yonumen.top/gtpqwddzgg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sufxvd.cn/gtxndrhjvl.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangkeji.top/gtucskndnq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.birdmap.top/gtfegaxasy.html

[R73] 分割大日志
来源：http://hz.zhijiandao.cn/gtyulismpj.html

split -l 1000 big.log part_
来源：http://hz.dianchejie.cn/gtxvryxmjs.html

[R74] 批量重命名
来源：http://hz.hfpthk.cn/gteptnttzc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtzivjzasn.html

[R75] 导出环境变量
来源：http://hz.zdqjudy.top/gtffdmzfag.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gtfnxnwchz.html

[R76] 使用临时文件
来源：http://hz.cheryme.top/gtrzzbfifl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.haohaochexian.top/gtezspagbd.html

[R77] 读取用户输入
来源：http://hz.quarkkingdee.top/gtdlqpqhwh.html

read -rp "请输入: " ans
来源：http://hz.quarkkingdee.top/gtzseobxap.html

[R78] 交互式菜单
来源：http://hz.daxiang520.top/gtwtpesqnb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhijiandao.cn/gtgetpogwh.html

[R79] 解析命令行选项
来源：http://hz.jyoumei.cn/gtmlhgease.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pycfn.com/gtxdrbttbj.html

[R80] 查看脚本执行耗时
来源：http://hz.jinghuilouyu.cn/gtkiaahnjm.html

time ./run.sh
来源：http://hz.vqdsnc.cn/gtllxojmbr.html

================================================================================
来源：http://hz.shzxlz.cn/gtfdcgyhin.html

S. C / C++ 专题
来源：http://hz.jinghuilouyu.cn/gtiucoddqn.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmdkdwwzn.html

[S01] C：Hello World
来源：http://hz.jianghu66.top/gtkmywjofv.html

#include <stdio.h>
来源：http://hz.wangdashe.top/gtcqydmijj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shangyingyoupin.top/gtyxfqwuhw.html

[S02] C：变量与格式化输出
来源：http://hz.bjfxy.top/gtzrhisghx.html

int a = 10; printf("%d\n", a);
来源：http://hz.cucudq.cn/gtgjotmxti.html

[S03] C：读入整数
来源：http://hz.svipenyu.cn/gtlmlhztbv.html

int x; scanf("%d", &x);
来源：http://hz.cqqwz.cn/gtipuovxvq.html

[S04] C：字符串复制
来源：http://hz.hnqzz.top/gtiyobvkvq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yangfankeji.com/gtmxasxydp.html

[S05] C：字符串长度
来源：http://hz.gaohongyu789.top/gtvzwhkduu.html

strlen(s)
来源：http://hz.birdmap.top/gttqxxvfcw.html

[S06] C：字符串比较
来源：http://hz.zhongyouzk.top/gttimorrjy.html

strcmp(a, b) == 0
来源：http://hz.xinyue.icu/gtmtaevgpt.html

[S07] C：数组遍历求和
来源：http://hz.jinqigufen.top/gtifskspae.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xingfuxueyuan.xyz/gtzfzcaxgf.html

[S08] C：动态内存分配与释放
来源：http://hz.xingfuxueyuan.xyz/gtcwtwzwvk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yanxiufei.cn/gthhujmghl.html

[S09] C：结构体定义与初始化
来源：http://hz.tanke756.top/gtkubqwsuz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aibaodan.cn/gtxfrtipwm.html

[S10] C：指针与解引用
来源：http://hz.yuxming.cn/gtpgzhqlhn.html

int *p = &a;  *p = 5;
来源：http://hz.pengpengdd.cyou/gteyxytsig.html

[S11] C：逐行读文件
来源：http://hz.jinqigufen.top/gteqoaegme.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydzc1.top/gtdsmcuyjc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gthfzdmdaf.html

fclose(f);
来源：http://hz.shanyushiyangtech.top/gtcouhiddq.html

[S12] C：写文件
来源：http://hz.cucudq.cn/gtlblhhvev.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtwrmbprnu.html

[S13] C：宏定义
来源：http://hz.zhongyouzk.top/gthpfdsyaq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guannengcc.top/gterpppqlt.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtmmafrccm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gotoacloud.top/gthzxjxdkq.html

[S15] C：类型转换
来源：http://hz.svipenyu.cn/gtsowgawsg.html

(double) a / b
来源：http://hz.jqgfzy.top/gteljvoaoi.html

[S16] C：位操作置位
来源：http://hz.hnxiangtu.top/gtpnpixyaa.html

x |= (1 << 3);
来源：http://hz.kuanghao11.cn/gtehfesrvh.html

[S17] C：安全拼接字符串
来源：http://hz.smart0.xyz/gtfvjqkted.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258888.top/gtcvndygwn.html

[S18] C：命令行参数
来源：http://hz.gogol.net.cn/gtzngczfbq.html

int main(int argc, char **argv)
来源：http://hz.ydzc1.top/gtmuzmwahc.html

[S19] C：快速排序
来源：http://hz.shanyushiyangtech.top/gtfmigrlki.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ydzc1.top/gtnhqcsryc.html

[S20] C：二分查找
来源：http://hz.yj20258.top/gtneigivlf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daxiang520.top/gthaksixcx.html

[S21] C：字符类别判断
来源：http://hz.ppjwa.cn/gtiypbghzp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shzxlz.cn/gtpkjkrhjt.html

[S22] C：字符串转数字
来源：http://hz.gotoacloud.top/gtknynzdbz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuxming.cn/gtcuyympab.html

[S23] C：随机数
来源：http://hz.cucudq.cn/gtblhgnysr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hammf.cn/gtkplopjai.html

[S24] C：获取本地时间
来源：http://hz.zhengqikj.top/gtpxatqlwt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigfzy.top/gtuiqivcmi.html

[S25] C：内存拷贝
来源：http://hz.wangdashe.top/gtnhtgxbyt.html

memcpy(dst, src, n);
来源：http://hz.zhoulong.xyz/gtoilmpogl.html

[S26] C：内存清零
来源：http://hz.zycfv.cn/gttykhmuvr.html

memset(a, 0, sizeof a);
来源：http://hz.zhengqikj.top/gtcnseqqen.html

[S27] C：定义常量
来源：http://hz.sysykeji.top/gthyqlqubl.html

const double PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtsbxqzqbe.html

[S28] C：静态变量
来源：http://hz.cheryme.top/gtyxeptjyr.html

static int counter = 0;
来源：http://hz.c1oappe.top/gtvtcausgl.html

[S29] C：变参函数
来源：http://hz.quarkkingdee.top/gtokaatqpm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtqioyzsyu.html

[S30] C：头文件保护
来源：http://hz.fzhhl.top/gtlbesrqqi.html

#ifndef X_H
来源：http://hz.cheryme.top/gtyeygqhvy.html

#define X_H
来源：http://hz.sysykeji.top/gtxxpxfsan.html

#endif
来源：http://hz.hongshengwenyu.top/gtxttuahfh.html

[S31] C++：Hello World
来源：http://hz.gotoacloud.top/gtlrmhcdio.html

#include <iostream>
来源：http://hz.wangdashe.top/gtpquktnmf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jiagoushi.top/gttruniqxa.html

[S32] C++：字符串
来源：http://hz.gaohongyu789.top/gtzxhzikfe.html

std::string s = "hi";  s += "!";
来源：http://hz.pycfn.com/gtfjlaywse.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangtech.top/gtqojkmtbg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hywenlv.cn/gtcnpbaeqh.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gtbmfceoxk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yanxiufei.cn/gtnhfzappi.html

[S35] C++：map
来源：http://hz.chenjidiqi.icu/gtkgoylylb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtajwrrbel.html

[S36] C++：unordered_map
来源：http://hz.sysykeji.top/gtgaacijhk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gtpanxxkhc.html

[S37] C++：set
来源：http://hz.0kj1m.cn/gtehphvzrm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xinyue.icu/gtkmifmyeu.html

[S38] C++：排序
来源：http://hz.quarkkingdee.top/gtebslofis.html

std::sort(v.begin(), v.end());
来源：http://hz.0kj1m.cn/gtjvkhuopm.html

[S39] C++：自定义比较器排序
来源：http://hz.yuxming.cn/gtcvgzznea.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tian-w.cn/gttxtmeqja.html

[S40] C++：查找元素
来源：http://hz.shzxlz.cn/gtcpmgaemh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shzxlz.cn/gtvfykfdpa.html

[S41] C++：类与构造函数
来源：http://hz.guannengcc.top/gthbuogomz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.9152youxi.cn/gtwhgjsjnz.html

[S42] C++：继承与虚函数
来源：http://hz.havefunace.top/gtbprbdflk.html

class B : public Base { public: void f() override {} };
来源：http://hz.jianghu66.top/gtihyaoxdl.html

[S43] C++：智能指针
来源：http://hz.pengpengdd.cyou/gtarxtkfvp.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtejdvuznh.html

[S44] C++：引用传参
来源：http://hz.bjfxy.top/gtivrczmvr.html

void inc(int &x) { ++x; }
来源：http://hz.zdqjudy.top/gtrcsdebgy.html

[S45] C++：lambda
来源：http://hz.jqgfzy.top/gtojltfwgk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cheryme.top/gtweqyuiuw.html

[S46] C++：函数模板
来源：http://hz.hfpthk.cn/gtwqawcunc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258888.top/gtcowjrnrr.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhoulong.xyz/gtwotqayzu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.meibo888.top/gtypbqyomm.html

[S48] C++：逐行读文件
来源：http://hz.cdnleiting.top/gtgmphdmfd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangshuangyany.cn/gtqsvrgklx.html

while (std::getline(in, line)) { }
来源：http://hz.smart0.xyz/gtdwjhdwxm.html

[S49] C++：写文件
来源：http://hz.nanxuanxn.top/gtsouqxmmc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daria6918.cn/gttnfjwkon.html

[S50] C++：格式化数字
来源：http://hz.meibo888.top/gtwysdrnak.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.wangdashe.top/gtndjwqyut.html

[S51] C++：显式类型转换
来源：http://hz.nanxuanxn.top/gttverwrqk.html

static_cast<double>(a) / b
来源：http://hz.52xcode.cn/gtdwvgtkjk.html

[S52] C++：const 与 noexcept
来源：http://hz.mhx1999.top/gtzfmttnuq.html

int size() const noexcept { return n_; }
来源：http://hz.zhoulong.xyz/gtfcfklqvj.html

[S53] C++：移动语义
来源：http://hz.zdqjudy.top/gtdtqhapwt.html

std::vector<int> w = std::move(v);
来源：http://hz.shuidangran.top/gtbvveurhy.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtsvtekaln.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tian-w.cn/gthmfdiokt.html

[S55] C++：结构化绑定
来源：http://hz.shuidangran.top/gtzgkccrbv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jianghu66.top/gtdvcqoxed.html

[S56] C++：optional
来源：http://hz.hongshengwenyu.top/gtzcgtfuoq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daria6918.cn/gtzbnbandf.html

[S57] C++：编译期常量
来源：http://hz.kuanghao11.cn/gtutlrzyrp.html

constexpr int N = 10;
来源：http://hz.nwbrower.top/gtmlbslkhj.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtczqqegaj.html

namespace ns { int f() { return 1; } }
来源：http://hz.cheryme.top/gtjiphhavi.html

[S59] C++：静态断言
来源：http://hz.xuetiantiany.cn/gtqehkijro.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xylfe.cn/gtkyqxvnwf.html

[S60] C++：遍历并删除元素
来源：http://hz.dashuyun.cn/gtsuptxsmk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ywan-chungtsiang.top/gtjlksihjk.html

================================================================================
来源：http://hz.hysaishi.cn/gtjkymfbaf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cdnleiting.top/gtikilxrvn.html

================================================================================
来源：http://hz.gzhubu.top/gtfgukpgry.html


<!-- 参考信息 -->