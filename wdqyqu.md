代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dashuyun.cn/gttcxxkdfz.html

[Q90] 生成序号列
来源：http://hz.nwbrower.top/gtkgqyxcrz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sxryk.cn/gtjgoosoec.html

================================================================================
来源：http://hz.tianlin.xyz/gtotwgvyje.html

R. Bash 专题
来源：http://hz.zhixingplan.top/gttruvfwfg.html

================================================================================
来源：http://hz.aizwys.cn/gthynfrjfh.html

[R01] shebang 与严格模式
来源：http://hz.smart0.xyz/gtxnrvqkre.html

#!/usr/bin/env bash
来源：http://hz.wangshuangyany.cn/gtxcrkvucv.html

set -euo pipefail
来源：http://hz.yj202588.top/gtjoxoaspn.html

[R02] 变量赋值与使用
来源：http://hz.yonumen.top/gtdsusbdqr.html

name="Tom"; echo "$name"
来源：http://hz.yongpay.top/gtbmphwtfa.html

[R03] 只读变量
来源：http://hz.jyoumei.cn/gtfvalaooq.html

readonly PI=3.14
来源：http://hz.dianchejie.cn/gtweihxojy.html

[R04] 位置参数
来源：http://hz.xuetiantiany.cn/gtnukuxrmm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shzxlz.cn/gtebfhthxf.html

[R05] 参数默认值
来源：http://hz.hfpthk.cn/gtklvhoykl.html

name="${1:-default}"
来源：http://hz.tianlin.xyz/gtiwznvpay.html

[R06] 判断命令是否存在
来源：http://hz.chenjidiqi.icu/gttrepwpva.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tianlin.xyz/gteamqkcfd.html

[R07] if 判断文件
来源：http://hz.jlsjyb.cn/gtpoxsoqtb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hfpthk.cn/gtvdxhohvb.html

[R08] 数值比较
来源：http://hz.xingfuxueyuan.xyz/gtvfntvqph.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangdashe.top/gtrawqhsqs.html

[R09] 字符串比较
来源：http://hz.aibaodan.cn/gtwtdviviq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ehwqpu.com/gtndvffcss.html

[R10] 正则匹配
来源：http://hz.52xcode.cn/gtthmwaueh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhijiandao.cn/gtvsrfpnut.html

[R11] case 多分支
来源：http://hz.chenzaomai.com/gtbpzcstzl.html

case "$1" in
来源：http://hz.hfpthk.cn/gtblaeprtc.html

start) echo "启动" ;;
来源：http://hz.xuanzx.com/gttwkmehbe.html

stop)  echo "停止" ;;
来源：http://hz.snrcjt.cn/gtqhjefpnp.html

*)     echo "未知命令" ;;
来源：http://hz.zhijiandao.cn/gtekkjieai.html

esac
来源：http://hz.bjfxy.top/gtleefmzxs.html

[R12] for 遍历文件
来源：http://hz.aibaodan.cn/gtunjkxwky.html

for f in *.txt; do echo "$f"; done
来源：http://hz.dianchejie.cn/gtfljvzseb.html

[R13] for 计数循环
来源：http://hz.chenzaomai.com/gtrurlopav.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cheryme.top/gtdgkngfrq.html

[R14] C 风格 for
来源：http://hz.hysaishi.cn/gtmgandppu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yonumen.top/gtpbtlqnel.html

[R15] while 逐行读文件
来源：http://hz.sxryk.cn/gtlfnfgbux.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ybcxt.top/gtdtochmkz.html

[R16] until 等待条件
来源：http://hz.snrcjt.cn/gtlrvfjmce.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.52xcode.cn/gtbwemrqsb.html

[R17] 数组定义与取值
来源：http://hz.kuanghao11.cn/gthjlzqgkn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sweek.top/gtyprsosut.html

[R18] 遍历数组
来源：http://hz.chenlongwang.top/gtskwzbzxb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.mhx1999.top/gtuxeupsnw.html

[R19] 数组长度
来源：http://hz.mhx1999.top/gtswxhjjqi.html

echo "${#arr[@]}"
来源：http://hz.quarkkingdee.top/gtziudczxz.html

[R20] 关联数组（字典）
来源：http://hz.yuxming.cn/gtwriziicn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.mhx1999.top/gtywefvsqq.html

[R21] 字符串长度
来源：http://hz.zhijiandao.cn/gttyyqflcu.html

echo "${#s}"
来源：http://hz.xylfe.cn/gtzutrsddc.html

[R22] 截取子串
来源：http://hz.pengpengdd.cyou/gtaoljaflf.html

echo "${s:0:5}"
来源：http://hz.shuidangran.top/gtgeubrycy.html

[R23] 字符串替换
来源：http://hz.xuetiantiany.cn/gtimnuubcq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sweek.top/gtmqbanbiq.html

[R24] 大小写转换
来源：http://hz.xziqi.cn/gtonqjkqgj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtdybfrzbd.html

[R25] 去后缀 / 去前缀
来源：http://hz.gogol.net.cn/gtwvkwovrp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gtyjgsehud.html

[R26] 命令替换
来源：http://hz.smart0.xyz/gtmyzqebwq.html

now=$(date +%F); echo "$now"
来源：http://hz.haohaochexian.top/gtyreivhtg.html

[R27] 算术展开
来源：http://hz.vqdsnc.cn/gtlznldeos.html

echo $((1 + 2 * 3))
来源：http://hz.gogol.net.cn/gterwppuqt.html

[R28] 浮点运算
来源：http://hz.ehwqpu.com/gtkaxfwlea.html

echo "scale=2; 10/3" | bc
来源：http://hz.xylfe.cn/gttgkmirxg.html

[R29] 定义函数
来源：http://hz.sweek.top/gtgglcktez.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yueranfly.top/gtschrjmhz.html

[R30] 函数返回状态码
来源：http://hz.guannengcc.top/gtxhspcauj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zdqjudy.top/gtmlfwbcby.html

[R31] 局部变量
来源：http://hz.cashguo.top/gtfliucrkm.html

f() { local x=1; echo "$x"; }
来源：http://hz.9152youxi.cn/gtcsgzghdc.html

[R32] 参数个数校验
来源：http://hz.gogol.net.cn/gtamshosyk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhoulong.xyz/gtgwhbugop.html

[R33] 捕获错误并提示行号
来源：http://hz.ywan-chungtsiang.top/gtiwybexcq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gzhubu.top/gtuvzgyvbq.html

[R34] 退出时清理
来源：http://hz.shanyushiyangkeji.top/gtwdbahqnt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtsqhcrhnv.html

[R35] 后台执行并等待
来源：http://hz.hongshengwenyu.top/gtojafukbo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hysaishi.cn/gtobuuyjxv.html

[R36] 并发执行多个任务
来源：http://hz.haohaochexian.top/gtiyibvnwi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cucudq.cn/gtrkaajqqi.html

[R37] 把输出赋给变量
来源：http://hz.hongshengwenyu.top/gtxdtqtkrs.html

files=$(ls -1)
来源：http://hz.hysaishi.cn/gtduknnhav.html

[R38] 管道串联
来源：http://hz.yj20258.top/gtjcrpfoqo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ivvv.top/gtwwmvjbgp.html

[R39] 重定向标准输出与错误
来源：http://hz.ydjk.org.cn/gtgcawlqbx.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangkeji.top/gtepwzjqhs.html

[R40] 追加写日志
来源：http://hz.hnqzz.top/gtodlfvqhf.html

echo "log" >> out.log
来源：http://hz.zhengqikj.top/gtpunhbgrd.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtrjneguuq.html

cmd >/dev/null 2>&1
来源：http://hz.vqdsnc.cn/gtuyndclpw.html

[R42] 输入重定向
来源：http://hz.chenjidiqi.icu/gtetoquxlr.html

wc -l < a.txt
来源：http://hz.ppjwa.cn/gtwrtcnhfb.html

[R43] 按名字查找文件
来源：http://hz.shuidangran.top/gtdytcneia.html

find . -name "*.log" -type f
来源：http://hz.hywenlv.cn/gtpjqqwfcc.html

[R44] 按修改时间查找
来源：http://hz.xuanzx.com/gtkjjnhzks.html

find . -mtime -7 -type f
来源：http://hz.jinyuanbaomall.cn/gtrenznstt.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gtsknisjgj.html

find . -name "*.tmp" -delete
来源：http://hz.svipenyu.cn/gtcmpetage.html

[R46] 递归替换文件内容
来源：http://hz.zycfv.cn/gtejtejlfe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gtpvwskwex.html

[R47] sed 单行替换
来源：http://hz.daria6918.cn/gtiydntajm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj202588.top/gtfvlyzxmo.html

[R48] awk 取指定列
来源：http://hz.chenlongwang.top/gtutwsndpo.html

awk '{print $1, $3}' a.txt
来源：http://hz.sufxvd.cn/gtwtgdbqzi.html

[R49] awk 带条件
来源：http://hz.ybcxt.top/gtekafbene.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.mhx1999.top/gtmtbenwjl.html

[R50] awk 求和
来源：http://hz.ydzc1.top/gtpxiptknd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yueranfly.top/gtwnxburdj.html

[R51] 排序去重取前几
来源：http://hz.fengsongda.top/gtoxltrjen.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.haohaochexian.top/gtbuurfipj.html

[R52] 统计行数
来源：http://hz.gotoacloud.top/gtluxawlbh.html

wc -l a.txt
来源：http://hz.shanyushiyangtech.top/gtdiagtvnw.html

[R53] 查看文件头与实时尾
来源：http://hz.aizwys.cn/gtesoxmket.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pycfn.com/gtxosvhfjx.html

[R54] 比较两个文件
来源：http://hz.redwolf501.top/gtnpxgebmy.html

diff a.txt b.txt
来源：http://hz.jinqigufen.top/gtykxjzfcn.html

[R55] 压缩与解压
来源：http://hz.hysaishi.cn/gtcgrdjffp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yueranfly.top/gtdfxndpvg.html

[R56] 远程拷贝
来源：http://hz.birdmap.top/gtudqnfnri.html

scp file user@host:/path/
来源：http://hz.jqgfzy.top/gtxuvibiok.html

[R57] 远程执行命令
来源：http://hz.cqqwz.cn/gtoxdqlncb.html

ssh user@host 'uptime'
来源：http://hz.jyoumei.cn/gtfsusfxdi.html

[R58] 下载文件
来源：http://hz.daxiang520.top/gtfyplpwld.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hongshengwenyu.top/gtrfowxtkd.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gtpcnbztpq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.daxiang520.top/gtriasqkwg.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtfpknhlao.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gzhubu.top/gtahuagzqh.html

[R61] 磁盘占用
来源：http://hz.zhiwuduotai.top/gthvuxbsqy.html

df -h;  du -sh *
来源：http://hz.zdqjudy.top/gtxeeiuaqy.html

[R62] 找最占空间的文件
来源：http://hz.jinqigfzy.top/gtedtjznlx.html

du -ah . | sort -rh | head -10
来源：http://hz.jlsjyb.cn/gtdukezpwx.html

[R63] 内存与进程
来源：http://hz.zhiwuduotai.top/gtbhpganbo.html

free -h;  ps aux | grep nginx
来源：http://hz.chenzaomai.com/gtduynwrvc.html

[R64] 结束进程
来源：http://hz.ppjwa.cn/gtsnndeinq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.kuanghao11.cn/gtulxzjhvf.html

[R65] 查看端口占用
来源：http://hz.mhx1999.top/gtluivxdhp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinghuilouyu.cn/gtrvsumtmi.html

[R66] 定时任务
来源：http://hz.hfpthk.cn/gtfjvhmrzl.html

crontab -e;  crontab -l
来源：http://hz.smart0.xyz/gtorwxxysp.html

[R67] 生成随机十六进制串
来源：http://hz.zhixingplan.top/gtpglebncl.html

openssl rand -hex 16
来源：http://hz.pycfn.com/gthbnpdtov.html

[R68] 计算文件校验值
来源：http://hz.xuanzx.com/gtevybkrhu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jlsjyb.cn/gtxoqwhzwg.html

[R69] 生成随机密码
来源：http://hz.iojbl.cn/gtzejtjtoc.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtkysyupyb.html

[R70] 时间戳与互转
来源：http://hz.ybcxt.top/gtbdkfmsvw.html

date +%s;  date -d @1700000000
来源：http://hz.chenjidiqi.icu/gtrrizrihy.html

[R71] 日期格式化
来源：http://hz.tanke756.top/gtjzcaqgfl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yueranfly.top/gtryryfqkp.html

[R72] 等待端口就绪
来源：http://hz.gotoacloud.top/gtuqwzycvt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shanyushiyangkeji.top/gtgonfvydt.html

[R73] 分割大日志
来源：http://hz.zhengqikj.top/gtohnjcpgo.html

split -l 1000 big.log part_
来源：http://hz.wangdashe.top/gtzftckxsk.html

[R74] 批量重命名
来源：http://hz.wangshuangyany.cn/gtmtvpgylt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhaomingkeji.xyz/gtopwxmjqn.html

[R75] 导出环境变量
来源：http://hz.haohaochexian.top/gtkjdotkqa.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ywan-chungtsiang.top/gtvxywlnhr.html

[R76] 使用临时文件
来源：http://hz.jlsjyb.cn/gtnxlgkymf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtlrxwyfnv.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gtlsugvvnc.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangtech.top/gtxnuydkas.html

[R78] 交互式菜单
来源：http://hz.jqgufenzy.top/gtpzywfcjg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydzc1.top/gtouhybiyn.html

[R79] 解析命令行选项
来源：http://hz.zhaomingkeji.xyz/gtuaqgjyox.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinqigufen.top/gtjvjrjnwq.html

[R80] 查看脚本执行耗时
来源：http://hz.yvedp.cn/gtdenmuafj.html

time ./run.sh
来源：http://hz.jqgufenzy.top/gtloagifpc.html

================================================================================
来源：http://hz.yvedp.cn/gtprudwezq.html

S. C / C++ 专题
来源：http://hz.meibo888.top/gtfwieyevp.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtgppedcih.html

[S01] C：Hello World
来源：http://hz.bjfxy.top/gtnbqtzkxm.html

#include <stdio.h>
来源：http://hz.cqqwz.cn/gtistdqseb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.redwolf501.top/gtinjldlby.html

[S02] C：变量与格式化输出
来源：http://hz.daxiang520.top/gtqbyamixh.html

int a = 10; printf("%d\n", a);
来源：http://hz.ivvv.top/gthbquraaj.html

[S03] C：读入整数
来源：http://hz.wangdashe.top/gtbrcwenwc.html

int x; scanf("%d", &x);
来源：http://hz.aibaodan.cn/gtykbjfpog.html

[S04] C：字符串复制
来源：http://hz.ydjk.org.cn/gtbowzualy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.52xcode.cn/gtphwijzld.html

[S05] C：字符串长度
来源：http://hz.aizwys.cn/gtogujaczq.html

strlen(s)
来源：http://hz.zhoulong.xyz/gthekupbsa.html

[S06] C：字符串比较
来源：http://hz.snrcjt.cn/gtvmxjgwse.html

strcmp(a, b) == 0
来源：http://hz.yongpay.top/gtbfrtwzts.html

[S07] C：数组遍历求和
来源：http://hz.fzhhl.top/gthgmlulzt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guannengcc.top/gtwccvhfmh.html

[S08] C：动态内存分配与释放
来源：http://hz.xylfe.cn/gtvcvewboo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ehwqpu.com/gtvthwlkhc.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258.top/gtcyaffoiw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.andypj.xyz/gtycqzelek.html

[S10] C：指针与解引用
来源：http://hz.yuxming.cn/gtpayilchl.html

int *p = &a;  *p = 5;
来源：http://hz.yueranfly.top/gtednrequy.html

[S11] C：逐行读文件
来源：http://hz.shuidangran.top/gtleheoatg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sxryk.cn/gtjvyqpboe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dianchejie.cn/gtsnjtjitl.html

fclose(f);
来源：http://hz.jianghu66.top/gtffkdjmzi.html

[S12] C：写文件
来源：http://hz.gotoacloud.top/gtainkqkim.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.haohaochexian.top/gtntgbxnkc.html

[S13] C：宏定义
来源：http://hz.316326.xyz/gtncqtggvw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xuetiantiany.cn/gtubnzvqez.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gtpgjprjub.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ywan-chungtsiang.top/gtfwryctjl.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtebhautqn.html

(double) a / b
来源：http://hz.hywenlv.cn/gtstubzelj.html

[S16] C：位操作置位
来源：http://hz.ydzc1.top/gtxggcmpwv.html

x |= (1 << 3);
来源：http://hz.yonumen.top/gtcndcrzlx.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258888.top/gtgugryffp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.guannengcc.top/gtfqeyhvbw.html

[S18] C：命令行参数
来源：http://hz.52xcode.cn/gtpbwdmhbt.html

int main(int argc, char **argv)
来源：http://hz.jinqigufen.top/gtnwbmcseb.html

[S19] C：快速排序
来源：http://hz.tian-w.cn/gtitpjrrgb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtqbuxusus.html

[S20] C：二分查找
来源：http://hz.tianlin.xyz/gttrqcrgau.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gtkxrfwvwq.html

[S21] C：字符类别判断
来源：http://hz.nanxinkj.top/gtasqlddkg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hywenlv.cn/gtptfaewuf.html

[S22] C：字符串转数字
来源：http://hz.ppjwa.cn/gttjboqkew.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guannengcc.top/gtcpitkmrc.html

[S23] C：随机数
来源：http://hz.hnxiangtu.top/gtmtldgatx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cdnleiting.top/gtactfrlpj.html

[S24] C：获取本地时间
来源：http://hz.cqqwz.cn/gttuvsnlbj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ppjwa.cn/gtgljerrgv.html

[S25] C：内存拷贝
来源：http://hz.jinyuanbaomall.cn/gtckueuayn.html

memcpy(dst, src, n);
来源：http://hz.c1oappe.top/gtobzjrvmm.html

[S26] C：内存清零
来源：http://hz.chenzaomai.com/gtwddxoywf.html

memset(a, 0, sizeof a);
来源：http://hz.dashuyun.cn/gtzshzocts.html

[S27] C：定义常量
来源：http://hz.gzhubu.top/gttajcshbv.html

const double PI = 3.14159;
来源：http://hz.pycfn.com/gtkbduraou.html

[S28] C：静态变量
来源：http://hz.0kj1m.cn/gtyrmordcs.html

static int counter = 0;
来源：http://hz.316326.xyz/gtazumyage.html

[S29] C：变参函数
来源：http://hz.shangyingyoupin.top/gtgbezhmsb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigufen.top/gtetxrmoyi.html

[S30] C：头文件保护
来源：http://hz.jqgfzy.top/gtugulomdy.html

#ifndef X_H
来源：http://hz.tian-w.cn/gtwtsugjwi.html

#define X_H
来源：http://hz.ehwqpu.com/gtpsbupojw.html

#endif
来源：http://hz.xingfuxueyuan.xyz/gtetbmmmma.html

[S31] C++：Hello World
来源：http://hz.jlsjyb.cn/gtekherxzk.html

#include <iostream>
来源：http://hz.cucudq.cn/gtdntvlphi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinghuilouyu.cn/gtnvzyawep.html

[S32] C++：字符串
来源：http://hz.316326.xyz/gtxnfnrjmb.html

std::string s = "hi";  s += "!";
来源：http://hz.nanxinkj.top/gtuwjiswow.html

[S33] C++：vector 增删
来源：http://hz.bjfxy.top/gtylogokzn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.dashuyun.cn/gtoqciiqwg.html

[S34] C++：遍历 vector
来源：http://hz.mhx1999.top/gttrtodpcg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.quarkkingdee.top/gtrzujbtym.html

[S35] C++：map
来源：http://hz.haohaochexian.top/gtvlzqxnnb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.vqdsnc.cn/gtcqfdnfov.html

[S36] C++：unordered_map
来源：http://hz.yj202588.top/gtzufopqhi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtoxsvuegv.html

[S37] C++：set
来源：http://hz.ydzc1.top/gtqowxkrnt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fzhhl.top/gtdthvwsfr.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtkmjufjos.html

std::sort(v.begin(), v.end());
来源：http://hz.ppjwa.cn/gtytaujlng.html

[S39] C++：自定义比较器排序
来源：http://hz.wangshuangyany.cn/gthaalmomr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yuxming.cn/gtxpnhqpag.html

[S40] C++：查找元素
来源：http://hz.chenzaomai.com/gtgvgodpbx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhongyouzk.top/gtdvtfbycu.html

[S41] C++：类与构造函数
来源：http://hz.9152youxi.cn/gtbqzoxxft.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nwbrower.top/gtrzywelan.html

[S42] C++：继承与虚函数
来源：http://hz.nwbrower.top/gtoxqdluzp.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhiwuduotai.top/gtibztcrbb.html

[S43] C++：智能指针
来源：http://hz.jinqigfzy.top/gtqulcvnil.html

auto p = std::make_unique<int>(5);
来源：http://hz.aizwys.cn/gttnsgtfoh.html

[S44] C++：引用传参
来源：http://hz.kuanghao11.cn/gtvuuhnuuw.html

void inc(int &x) { ++x; }
来源：http://hz.daria6918.cn/gtzhjdfdku.html

[S45] C++：lambda
来源：http://hz.shuidangran.top/gtxprevjme.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.quarkkingdee.top/gtsowdgfym.html

[S46] C++：函数模板
来源：http://hz.yanxiufei.cn/gtfvaahtyu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhijiandao.cn/gtiqrirjom.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gthmrnfquf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shzxlz.cn/gtmibewsld.html

[S48] C++：逐行读文件
来源：http://hz.zdqjudy.top/gtzsuzkpvr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.meibo888.top/gtaenhoccs.html

while (std::getline(in, line)) { }
来源：http://hz.jinghuilouyu.cn/gtfkeounkv.html

[S49] C++：写文件
来源：http://hz.zdqjudy.top/gtvfbvvcow.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtkzjothcw.html

[S50] C++：格式化数字
来源：http://hz.sweek.top/gtqcttucdp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtpqauyaeh.html

[S51] C++：显式类型转换
来源：http://hz.ehwqpu.com/gtwektuiky.html

static_cast<double>(a) / b
来源：http://hz.tianlin.xyz/gtneabhlug.html

[S52] C++：const 与 noexcept
来源：http://hz.xuetiantiany.cn/gtgxgjiegz.html

int size() const noexcept { return n_; }
来源：http://hz.ydzc1.top/gtsddlsevb.html

[S53] C++：移动语义
来源：http://hz.hysaishi.cn/gtueahgdql.html

std::vector<int> w = std::move(v);
来源：http://hz.jlsjyb.cn/gtwujvhysk.html

[S54] C++：异常处理
来源：http://hz.gzhubu.top/gtkdoolndr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hfpthk.cn/gtvwefbrqt.html

[S55] C++：结构化绑定
来源：http://hz.aibaodan.cn/gtboxevkcg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tian-w.cn/gtuazrejuj.html

[S56] C++：optional
来源：http://hz.0kj1m.cn/gtpjxgjpng.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ivvv.top/gtjlwpxfob.html

[S57] C++：编译期常量
来源：http://hz.jinqigfzy.top/gtknyfmmja.html

constexpr int N = 10;
来源：http://hz.bjfxy.top/gtyjqhirnb.html

[S58] C++：命名空间
来源：http://hz.zdqjudy.top/gtsgszxscm.html

namespace ns { int f() { return 1; } }
来源：http://hz.yanxiufei.cn/gtmxjvlwbc.html

[S59] C++：静态断言
来源：http://hz.chenzaomai.com/gtffufpxtu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.c1oappe.top/gtvbngngmx.html

[S60] C++：遍历并删除元素
来源：http://hz.ybcxt.top/gtakagjpnf.html


<!-- 参考信息 -->