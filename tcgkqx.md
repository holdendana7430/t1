代发 wailian999

R. Bash 专题
来源：http://hz.gogol.net.cn/gtxfzekdhu.html

================================================================================
来源：http://hz.dashuyun.cn/gtgrvcyqob.html

[R01] shebang 与严格模式
来源：http://hz.daria6918.cn/gttfpdlpmk.html

#!/usr/bin/env bash
来源：http://hz.sxryk.cn/gtrxqmlpev.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtjpzhvweu.html

[R02] 变量赋值与使用
来源：http://hz.shangyingyoupin.top/gtpmjxpequ.html

name="Tom"; echo "$name"
来源：http://hz.pengpengdd.cyou/gtcmcmuojn.html

[R03] 只读变量
来源：http://hz.yuxming.cn/gtggzaugnx.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtmykmdqrd.html

[R04] 位置参数
来源：http://hz.ivvv.top/gttirdxmin.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.feifeiyinyue.top/gttvnsrjqj.html

[R05] 参数默认值
来源：http://hz.daxiang520.top/gtmwiazaxf.html

name="${1:-default}"
来源：http://hz.hfpthk.cn/gtipmqlnjv.html

[R06] 判断命令是否存在
来源：http://hz.hfpthk.cn/gtblakbqnq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sweek.top/gtigaaflci.html

[R07] if 判断文件
来源：http://hz.daxiang520.top/gtuepgsslk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.smart0.xyz/gtqyzjsthc.html

[R08] 数值比较
来源：http://hz.zhijiandao.cn/gtqoedpxta.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.meibo888.top/gthidddghs.html

[R09] 字符串比较
来源：http://hz.mhx1999.top/gtoqgkvakq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hfpthk.cn/gtmsnbqufd.html

[R10] 正则匹配
来源：http://hz.sxryk.cn/gthjuhfzrj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shangyingyoupin.top/gtwjwkvdkc.html

[R11] case 多分支
来源：http://hz.0kj1m.cn/gtsekvdejl.html

case "$1" in
来源：http://hz.yueranfly.top/gtbkvgijam.html

start) echo "启动" ;;
来源：http://hz.hywenlv.cn/gtieahnetm.html

stop)  echo "停止" ;;
来源：http://hz.daxiang520.top/gtcgqxwsxy.html

*)     echo "未知命令" ;;
来源：http://hz.gaohongyu789.top/gtklyjjsbi.html

esac
来源：http://hz.iojbl.cn/gtujarqpkp.html

[R12] for 遍历文件
来源：http://hz.yueranfly.top/gtuydilsea.html

for f in *.txt; do echo "$f"; done
来源：http://hz.iojbl.cn/gtobgdenbm.html

[R13] for 计数循环
来源：http://hz.nanxuanxn.top/gtznyivfes.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.andypj.xyz/gtvqfjrczm.html

[R14] C 风格 for
来源：http://hz.jinyuanbaomall.cn/gtuyjthqur.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtnevuxesk.html

[R15] while 逐行读文件
来源：http://hz.yj20258888.top/gtpgnwkoho.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydjk.org.cn/gtljvstdeh.html

[R16] until 等待条件
来源：http://hz.chenlongwang.top/gtlxgwlrwv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgfzy.top/gtdecjcklf.html

[R17] 数组定义与取值
来源：http://hz.316326.xyz/gtdtknrtmz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.havefunace.top/gtwsveqfsu.html

[R18] 遍历数组
来源：http://hz.yvedp.cn/gttjovkezh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.smart0.xyz/gthnqfucok.html

[R19] 数组长度
来源：http://hz.ydjk.org.cn/gtccpvvyuu.html

echo "${#arr[@]}"
来源：http://hz.xinyue.icu/gtmfdutqnn.html

[R20] 关联数组（字典）
来源：http://hz.hfpthk.cn/gtvdoxkygv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.dianchejie.cn/gtolnhzvwr.html

[R21] 字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtlrlrulho.html

echo "${#s}"
来源：http://hz.jinyuanbaomall.cn/gtvnmdxmif.html

[R22] 截取子串
来源：http://hz.hysaishi.cn/gtmvmxuctj.html

echo "${s:0:5}"
来源：http://hz.yongpay.top/gtedrlhirm.html

[R23] 字符串替换
来源：http://hz.bjfxy.top/gtygzxkwpw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.316326.xyz/gtrsfnwzlp.html

[R24] 大小写转换
来源：http://hz.hammf.cn/gtdpvlqesu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhiwuduotai.top/gtsvfxofmu.html

[R25] 去后缀 / 去前缀
来源：http://hz.fengsongda.top/gtbsgtmzgu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.snrcjt.cn/gtzifcuccw.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtxbzrhnyj.html

now=$(date +%F); echo "$now"
来源：http://hz.c1oappe.top/gtgknlhrpu.html

[R27] 算术展开
来源：http://hz.dashuyun.cn/gtgejyhsqz.html

echo $((1 + 2 * 3))
来源：http://hz.zhijiandao.cn/gtqtgquxsa.html

[R28] 浮点运算
来源：http://hz.meibo888.top/gtlbjpwkvt.html

echo "scale=2; 10/3" | bc
来源：http://hz.vqdsnc.cn/gtgsleufub.html

[R29] 定义函数
来源：http://hz.gogol.net.cn/gtyotlnvpj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtifjnfkvw.html

[R30] 函数返回状态码
来源：http://hz.havefunace.top/gtibboaccc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xingfuxueyuan.xyz/gtfkzizayy.html

[R31] 局部变量
来源：http://hz.tian-w.cn/gtovglxuvi.html

f() { local x=1; echo "$x"; }
来源：http://hz.birdmap.top/gtpgyvwpjz.html

[R32] 参数个数校验
来源：http://hz.jinghuilouyu.cn/gtwycvihcl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xziqi.cn/gttztbzjhe.html

[R33] 捕获错误并提示行号
来源：http://hz.ppjwa.cn/gtsfyzvzdn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydzc1.top/gtxqspboqi.html

[R34] 退出时清理
来源：http://hz.wangshuangyany.cn/gtplzrzqvv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtxjonkzot.html

[R35] 后台执行并等待
来源：http://hz.zhoulong.xyz/gtxjsnsthv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xylfe.cn/gtfpclfdtk.html

[R36] 并发执行多个任务
来源：http://hz.vqdsnc.cn/gtxbxqsbjx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pengpengdd.cyou/gtvweubutv.html

[R37] 把输出赋给变量
来源：http://hz.sweek.top/gtkajnmmmn.html

files=$(ls -1)
来源：http://hz.cheryme.top/gtkbijueva.html

[R38] 管道串联
来源：http://hz.yanxiufei.cn/gtxkgtibus.html

cat a.txt | grep -i error | wc -l
来源：http://hz.316326.xyz/gtyrrkfins.html

[R39] 重定向标准输出与错误
来源：http://hz.jiagoushi.top/gtipwbfbte.html

cmd > out.log 2>&1
来源：http://hz.316326.xyz/gtjpewuien.html

[R40] 追加写日志
来源：http://hz.zhengqikj.top/gtdbwuzgkp.html

echo "log" >> out.log
来源：http://hz.jyoumei.cn/gtlwqqvxho.html

[R41] 丢弃输出
来源：http://hz.jinyuanbaomall.cn/gtutkzdcry.html

cmd >/dev/null 2>&1
来源：http://hz.zhiwuduotai.top/gtgzbwdiwi.html

[R42] 输入重定向
来源：http://hz.pycfn.com/gtkgvjwipz.html

wc -l < a.txt
来源：http://hz.ehwqpu.com/gtqrzdcfbh.html

[R43] 按名字查找文件
来源：http://hz.havefunace.top/gtjpzrorhh.html

find . -name "*.log" -type f
来源：http://hz.aizwys.cn/gtrcmukfly.html

[R44] 按修改时间查找
来源：http://hz.aizwys.cn/gtpwwtuckm.html

find . -mtime -7 -type f
来源：http://hz.jianghu66.top/gtfhcqecja.html

[R45] 批量删除
来源：http://hz.redwolf501.top/gtqtayohsh.html

find . -name "*.tmp" -delete
来源：http://hz.kuanghao11.cn/gtqjkuhunk.html

[R46] 递归替换文件内容
来源：http://hz.jianghu66.top/gtutytfkqw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ybcxt.top/gtduflpxwn.html

[R47] sed 单行替换
来源：http://hz.nanxinkj.top/gtipahqldc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fzhhl.top/gtwipogkji.html

[R48] awk 取指定列
来源：http://hz.sysykeji.top/gtmeratcnh.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuanzx.com/gtnwwxmytf.html

[R49] awk 带条件
来源：http://hz.shangyingyoupin.top/gtenysyrtl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258.top/gtdoqnabwu.html

[R50] awk 求和
来源：http://hz.xylfe.cn/gtkjmroulj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangtech.top/gtqdorfemj.html

[R51] 排序去重取前几
来源：http://hz.haohaochexian.top/gtjbdpcemo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhiwuduotai.top/gtbmyxcajc.html

[R52] 统计行数
来源：http://hz.ybcxt.top/gtujxwrgmp.html

wc -l a.txt
来源：http://hz.fzhhl.top/gtfgkvcqfs.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gtgrpinggs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtqojmltpo.html

[R54] 比较两个文件
来源：http://hz.0kj1m.cn/gthbwivbll.html

diff a.txt b.txt
来源：http://hz.ppjwa.cn/gtktkhpqll.html

[R55] 压缩与解压
来源：http://hz.ydzc1.top/gttrcnsmyk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenlongwang.top/gtkczjdbpu.html

[R56] 远程拷贝
来源：http://hz.haohaochexian.top/gtrgduaqwy.html

scp file user@host:/path/
来源：http://hz.316326.xyz/gtytlxlkbi.html

[R57] 远程执行命令
来源：http://hz.iojbl.cn/gtyvksqkel.html

ssh user@host 'uptime'
来源：http://hz.andypj.xyz/gtugaawhza.html

[R58] 下载文件
来源：http://hz.316326.xyz/gtyufxrktt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jlsjyb.cn/gtqmidclgk.html

[R59] 发 POST JSON
来源：http://hz.jinqigfzy.top/gtelhbsdlc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhijiandao.cn/gtimmmdmfw.html

[R60] 只看 HTTP 状态码
来源：http://hz.nwbrower.top/gtdkztmtsr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.c1oappe.top/gtfuspjgcf.html

[R61] 磁盘占用
来源：http://hz.ydjk.org.cn/gthufkctln.html

df -h;  du -sh *
来源：http://hz.haohaochexian.top/gtdmgfvbro.html

[R62] 找最占空间的文件
来源：http://hz.zhoulong.xyz/gtajidqawv.html

du -ah . | sort -rh | head -10
来源：http://hz.yangfankeji.com/gtxxhobgee.html

[R63] 内存与进程
来源：http://hz.gogol.net.cn/gtlycqpypx.html

free -h;  ps aux | grep nginx
来源：http://hz.iojbl.cn/gtgeardkel.html

[R64] 结束进程
来源：http://hz.tanke756.top/gtiwnbagaf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhongyouzk.top/gthltnfssi.html

[R65] 查看端口占用
来源：http://hz.hongshengwenyu.top/gtvjmqaxba.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gotoacloud.top/gtgpyrwrlx.html

[R66] 定时任务
来源：http://hz.zhixingplan.top/gtkwsrjvis.html

crontab -e;  crontab -l
来源：http://hz.yanxiufei.cn/gtihodpryf.html

[R67] 生成随机十六进制串
来源：http://hz.hnxiangtu.top/gtfskxcifk.html

openssl rand -hex 16
来源：http://hz.guowangkeji.top/gtxfzlswkm.html

[R68] 计算文件校验值
来源：http://hz.jlsjyb.cn/gtlszpfatr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xinyue.icu/gtchzuawjr.html

[R69] 生成随机密码
来源：http://hz.yuanzhike.top/gtasguzamh.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gthkixqiwi.html

[R70] 时间戳与互转
来源：http://hz.xuetiantiany.cn/gtrhcaazhn.html

date +%s;  date -d @1700000000
来源：http://hz.pycfn.com/gtyicihxkl.html

[R71] 日期格式化
来源：http://hz.yuxming.cn/gtigxdczwl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gotoacloud.top/gtidlpjsak.html

[R72] 等待端口就绪
来源：http://hz.52xcode.cn/gttmiolnrl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtrphcmixe.html

[R73] 分割大日志
来源：http://hz.vqdsnc.cn/gtqkzvmicc.html

split -l 1000 big.log part_
来源：http://hz.xingfuxueyuan.xyz/gtwenfreeq.html

[R74] 批量重命名
来源：http://hz.meibo888.top/gtxkysyimo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.c1oappe.top/gtbcwyhpnh.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gtpuntdwvv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jlsjyb.cn/gtvmoitqyz.html

[R76] 使用临时文件
来源：http://hz.nwbrower.top/gtamdyywzs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gttkwpwqqn.html

[R77] 读取用户输入
来源：http://hz.gotoacloud.top/gtqwnnxagd.html

read -rp "请输入: " ans
来源：http://hz.ivvv.top/gtchrgdoro.html

[R78] 交互式菜单
来源：http://hz.havefunace.top/gtufblawem.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.c1oappe.top/gtbsjeuajg.html

[R79] 解析命令行选项
来源：http://hz.mhx1999.top/gtcxkluyme.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jyoumei.cn/gtwsdpoddo.html

[R80] 查看脚本执行耗时
来源：http://hz.yonumen.top/gttqgmuinz.html

time ./run.sh
来源：http://hz.yj202588.top/gtoopmrhcm.html

================================================================================
来源：http://hz.cqqwz.cn/gtrytajcpn.html

S. C / C++ 专题
来源：http://hz.shanyushiyangkeji.top/gtkdpcdiru.html

================================================================================
来源：http://hz.yj20258.top/gtbzkzavgo.html

[S01] C：Hello World
来源：http://hz.feifeiyinyue.top/gtpddtlhuq.html

#include <stdio.h>
来源：http://hz.iojbl.cn/gtkeanukuk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hywenlv.cn/gtzhamezcq.html

[S02] C：变量与格式化输出
来源：http://hz.birdmap.top/gtnoauedov.html

int a = 10; printf("%d\n", a);
来源：http://hz.cqqwz.cn/gtmevhrfig.html

[S03] C：读入整数
来源：http://hz.yonumen.top/gtgjjwwibh.html

int x; scanf("%d", &x);
来源：http://hz.nwbrower.top/gtolvkjdhz.html

[S04] C：字符串复制
来源：http://hz.vqdsnc.cn/gtywqflqnt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.havefunace.top/gtzpjtmrrc.html

[S05] C：字符串长度
来源：http://hz.cheryme.top/gtvyhgaaac.html

strlen(s)
来源：http://hz.yuxming.cn/gtofwqshjm.html

[S06] C：字符串比较
来源：http://hz.xingfuxueyuan.xyz/gtgbitoqoq.html

strcmp(a, b) == 0
来源：http://hz.tianlin.xyz/gtuwddtdfa.html

[S07] C：数组遍历求和
来源：http://hz.chenzaomai.com/gtahillflh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yangfankeji.com/gtdlpbpjoz.html

[S08] C：动态内存分配与释放
来源：http://hz.gogol.net.cn/gtkdbrzhug.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.meibo888.top/gtjsszdunb.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gtmpshfqhh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gzhubu.top/gtjqzvwrca.html

[S10] C：指针与解引用
来源：http://hz.cashguo.top/gtsdhqezdt.html

int *p = &a;  *p = 5;
来源：http://hz.ivvv.top/gtuovnxskc.html

[S11] C：逐行读文件
来源：http://hz.hywenlv.cn/gtepnagypw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydzc1.top/gtszxookwa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xuanzx.com/gtsqwvqmzq.html

fclose(f);
来源：http://hz.jinghuilouyu.cn/gtcpgilsdd.html

[S12] C：写文件
来源：http://hz.quarkkingdee.top/gtcshllhzi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenjidiqi.icu/gtykftcsln.html

[S13] C：宏定义
来源：http://hz.sufxvd.cn/gthwloqgyk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhijiandao.cn/gtpcmlqabl.html

[S14] C：枚举
来源：http://hz.xingfuxueyuan.xyz/gtczkyvffx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.52xcode.cn/gtagtupfgi.html

[S15] C：类型转换
来源：http://hz.yonumen.top/gtuxndpfgv.html

(double) a / b
来源：http://hz.dashuyun.cn/gtwmwyqywe.html

[S16] C：位操作置位
来源：http://hz.shangyingyoupin.top/gtbvynkyxf.html

x |= (1 << 3);
来源：http://hz.ydjk.org.cn/gtitphrkqk.html

[S17] C：安全拼接字符串
来源：http://hz.gzhubu.top/gteselzrau.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.kuanghao11.cn/gtrhwzdpkp.html

[S18] C：命令行参数
来源：http://hz.ybcxt.top/gtbhizwwnj.html

int main(int argc, char **argv)
来源：http://hz.andypj.xyz/gtmzywedok.html

[S19] C：快速排序
来源：http://hz.yuanzhike.top/gtrsmyfusn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtmlxbbpms.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtabtvxjpq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgfzy.top/gtmkyucrlk.html

[S21] C：字符类别判断
来源：http://hz.c1oappe.top/gtppgmosmz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xuetiantiany.cn/gtzhvsdjib.html

[S22] C：字符串转数字
来源：http://hz.yj202588.top/gtpnrqrngd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.smart0.xyz/gtqnxzuotb.html

[S23] C：随机数
来源：http://hz.haohaochexian.top/gtylatqxcl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.tian-w.cn/gtnbikvdjc.html

[S24] C：获取本地时间
来源：http://hz.gzhubu.top/gtgismimtp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yongpay.top/gteehnugns.html

[S25] C：内存拷贝
来源：http://hz.birdmap.top/gtpuushnuj.html

memcpy(dst, src, n);
来源：http://hz.zhongyouzk.top/gtflhnvedo.html

[S26] C：内存清零
来源：http://hz.gogol.net.cn/gtwsnzvrdv.html

memset(a, 0, sizeof a);
来源：http://hz.316326.xyz/gttelpkqjw.html

[S27] C：定义常量
来源：http://hz.aizwys.cn/gtuvufaomi.html

const double PI = 3.14159;
来源：http://hz.sufxvd.cn/gtnszvyhyn.html

[S28] C：静态变量
来源：http://hz.redwolf501.top/gtfwydqolz.html

static int counter = 0;
来源：http://hz.ybcxt.top/gttvwaejun.html

[S29] C：变参函数
来源：http://hz.shanyushiyangtech.top/gttwyoecsl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yvedp.cn/gtnryxfmgm.html

[S30] C：头文件保护
来源：http://hz.cashguo.top/gtwbepqodq.html

#ifndef X_H
来源：http://hz.hammf.cn/gttrfhihqy.html

#define X_H
来源：http://hz.zhengqikj.top/gtbsmpoqow.html

#endif
来源：http://hz.zhijiandao.cn/gtzvbwynvl.html

[S31] C++：Hello World
来源：http://hz.yuxming.cn/gtxgnidvfe.html

#include <iostream>
来源：http://hz.yvedp.cn/gtjokgpton.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj202588.top/gtyaisrxty.html

[S32] C++：字符串
来源：http://hz.snrcjt.cn/gtcarvrjcy.html

std::string s = "hi";  s += "!";
来源：http://hz.yangfankeji.com/gtmxcmwnzk.html

[S33] C++：vector 增删
来源：http://hz.jiagoushi.top/gtnbdxeyxp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nwbrower.top/gtmuraboxv.html

[S34] C++：遍历 vector
来源：http://hz.zhengqikj.top/gtevcjcymq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jiagoushi.top/gtseegolrd.html

[S35] C++：map
来源：http://hz.nanxinkj.top/gtlaisasiw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtrflgtwca.html

[S36] C++：unordered_map
来源：http://hz.daria6918.cn/gtcmqfijet.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtlgrdycul.html

[S37] C++：set
来源：http://hz.yvedp.cn/gtoeqfyuli.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jyoumei.cn/gtifxbarpb.html

[S38] C++：排序
来源：http://hz.yj20258888.top/gtbsxjommb.html

std::sort(v.begin(), v.end());
来源：http://hz.guannengcc.top/gtbxtglzja.html

[S39] C++：自定义比较器排序
来源：http://hz.nanxinkj.top/gtoidcaggr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnxiangtu.top/gtruzeofyw.html

[S40] C++：查找元素
来源：http://hz.ydjk.org.cn/gtvjluirit.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shanyushiyangkeji.top/gtryaarqdb.html

[S41] C++：类与构造函数
来源：http://hz.wangdashe.top/gtpswibpjf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgufenzy.top/gttowgvryu.html

[S42] C++：继承与虚函数
来源：http://hz.tanke756.top/gtggzseicw.html

class B : public Base { public: void f() override {} };
来源：http://hz.cheryme.top/gtbcaltrbm.html

[S43] C++：智能指针
来源：http://hz.yj202588.top/gtsvghiptm.html

auto p = std::make_unique<int>(5);
来源：http://hz.feifeiyinyue.top/gtbqgpvinm.html

[S44] C++：引用传参
来源：http://hz.quarkkingdee.top/gtuokpuctb.html

void inc(int &x) { ++x; }
来源：http://hz.hnxiangtu.top/gtazgbecbl.html

[S45] C++：lambda
来源：http://hz.xylfe.cn/gtaanxfhbq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gaohongyu789.top/gtmgwgwwvy.html

[S46] C++：函数模板
来源：http://hz.yj20258.top/gtkmwcsoyw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtbfxpbhns.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhiwuduotai.top/gthuvvcaqd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yuanzhike.top/gtrgxoyced.html

[S48] C++：逐行读文件
来源：http://hz.daxiang520.top/gtsxmxixhq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydjk.org.cn/gtyswdlfzg.html

while (std::getline(in, line)) { }
来源：http://hz.nanxinkj.top/gtowqjwdaj.html

[S49] C++：写文件
来源：http://hz.xuetiantiany.cn/gtbkymbcdn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tian-w.cn/gtpvuutymi.html

[S50] C++：格式化数字
来源：http://hz.jlsjyb.cn/gtfuboschg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258888.top/gtsumxwwvx.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtpckqthmz.html

static_cast<double>(a) / b
来源：http://hz.cucudq.cn/gtkwzyrwnj.html

[S52] C++：const 与 noexcept
来源：http://hz.sweek.top/gttudswddd.html

int size() const noexcept { return n_; }
来源：http://hz.smart0.xyz/gtykftqwmv.html

[S53] C++：移动语义
来源：http://hz.redwolf501.top/gtbyiintsy.html

std::vector<int> w = std::move(v);
来源：http://hz.wangdashe.top/gtiwfmegsn.html

[S54] C++：异常处理
来源：http://hz.haohaochexian.top/gtedkfywfc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yueranfly.top/gtakxkccyx.html

[S55] C++：结构化绑定
来源：http://hz.tanke756.top/gtqogisunj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sysykeji.top/gtdchamgfb.html

[S56] C++：optional
来源：http://hz.yj20258888.top/gtdxmixiou.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj202588.top/gtwbpkdnyh.html

[S57] C++：编译期常量
来源：http://hz.yanxiufei.cn/gtsoviaxrl.html

constexpr int N = 10;
来源：http://hz.xinyue.icu/gtoroogncb.html

[S58] C++：命名空间
来源：http://hz.fzhhl.top/gtwlzhachf.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj20258.top/gtqpeoefum.html

[S59] C++：静态断言
来源：http://hz.wangdashe.top/gtoilfucgy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gogol.net.cn/gtphotrgtt.html

[S60] C++：遍历并删除元素
来源：http://hz.yuxming.cn/gtewxqwkyv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tanke756.top/gtjkxwjpnj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtnshsdgod.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhoulong.xyz/gtpljiumuo.html

================================================================================
来源：http://hz.hysaishi.cn/gtwblrygvd.html


<!-- 参考信息 -->