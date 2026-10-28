代发 wailian999

R. Bash 专题
来源：http://hz.guannengcc.top/gtghmivltq.html

================================================================================
来源：http://hz.nanxuanxn.top/gtgtnashcs.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtkwaozroe.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtqcnvuopo.html

set -euo pipefail
来源：http://hz.cheryme.top/gtnplathus.html

[R02] 变量赋值与使用
来源：http://hz.chenzaomai.com/gtjarlbtrl.html

name="Tom"; echo "$name"
来源：http://hz.kuanghao11.cn/gtgpviiedx.html

[R03] 只读变量
来源：http://hz.0kj1m.cn/gtzgjqkxsn.html

readonly PI=3.14
来源：http://hz.chenlongwang.top/gtfhyjxnoo.html

[R04] 位置参数
来源：http://hz.hfpthk.cn/gtvlrcssbw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yanxiufei.cn/gtlwwaxsbt.html

[R05] 参数默认值
来源：http://hz.ybcxt.top/gtabcskphw.html

name="${1:-default}"
来源：http://hz.sufxvd.cn/gtqifxvvdu.html

[R06] 判断命令是否存在
来源：http://hz.haohaochexian.top/gtpbrinaab.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shuidangran.top/gteycimfoz.html

[R07] if 判断文件
来源：http://hz.tanke756.top/gtypkcpqyt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xylfe.cn/gtlykuzwpc.html

[R08] 数值比较
来源：http://hz.xinyue.icu/gtmzulobbt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gttmjeigoz.html

[R09] 字符串比较
来源：http://hz.jinghuilouyu.cn/gtojtkhero.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.snrcjt.cn/gtgvzijcub.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtesmdcobo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tianlin.xyz/gtbnijjumq.html

[R11] case 多分支
来源：http://hz.cheryme.top/gtusslzhru.html

case "$1" in
来源：http://hz.xingfuxueyuan.xyz/gtrwkmujcx.html

start) echo "启动" ;;
来源：http://hz.ydjk.org.cn/gtgnkildnb.html

stop)  echo "停止" ;;
来源：http://hz.jqgfzy.top/gtbgeesmdd.html

*)     echo "未知命令" ;;
来源：http://hz.nanxinkj.top/gtrqtcrkwn.html

esac
来源：http://hz.dianchejie.cn/gtglkmqepn.html

[R12] for 遍历文件
来源：http://hz.aizwys.cn/gtrjtgjdhs.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgfzy.top/gtjwrvdond.html

[R13] for 计数循环
来源：http://hz.tian-w.cn/gtezesfybb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aizwys.cn/gtzyxcttle.html

[R14] C 风格 for
来源：http://hz.hongshengwenyu.top/gtqjnlneau.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gtxsceaeay.html

[R15] while 逐行读文件
来源：http://hz.ivvv.top/gtmpfgibze.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guannengcc.top/gteenyhzao.html

[R16] until 等待条件
来源：http://hz.dashuyun.cn/gtsbsexkck.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgufenzy.top/gttmbyoozg.html

[R17] 数组定义与取值
来源：http://hz.zhixingplan.top/gtsbaimoki.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.mhx1999.top/gtslcpzorx.html

[R18] 遍历数组
来源：http://hz.chenjidiqi.icu/gtupqbsyhb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yongpay.top/gtdqydezzn.html

[R19] 数组长度
来源：http://hz.kuanghao11.cn/gtmnqodpmv.html

echo "${#arr[@]}"
来源：http://hz.jinqigufen.top/gttgwepnlv.html

[R20] 关联数组（字典）
来源：http://hz.gaohongyu789.top/gthiedoaad.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhaomingkeji.xyz/gtgbybeoeq.html

[R21] 字符串长度
来源：http://hz.hnqzz.top/gtzddhjtva.html

echo "${#s}"
来源：http://hz.xuanzx.com/gturacinpo.html

[R22] 截取子串
来源：http://hz.nwbrower.top/gtgifqzezj.html

echo "${s:0:5}"
来源：http://hz.nanxinkj.top/gtbgpitqid.html

[R23] 字符串替换
来源：http://hz.zhijiandao.cn/gtqfpelgqa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yongpay.top/gtgphpjloy.html

[R24] 大小写转换
来源：http://hz.gzhubu.top/gthszwwctn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jqgfzy.top/gtffrnoxlz.html

[R25] 去后缀 / 去前缀
来源：http://hz.sweek.top/gtgiuhetdg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shzxlz.cn/gtfwvllrxs.html

[R26] 命令替换
来源：http://hz.yanxiufei.cn/gthtdyrlwj.html

now=$(date +%F); echo "$now"
来源：http://hz.shuidangran.top/gtattxppfi.html

[R27] 算术展开
来源：http://hz.iojbl.cn/gtkkyovqvd.html

echo $((1 + 2 * 3))
来源：http://hz.kuanghao11.cn/gtbphbtnif.html

[R28] 浮点运算
来源：http://hz.zhaomingkeji.xyz/gtmbgiaaqg.html

echo "scale=2; 10/3" | bc
来源：http://hz.cqqwz.cn/gtyosflopm.html

[R29] 定义函数
来源：http://hz.kuanghao11.cn/gtkbqnoxje.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.quarkkingdee.top/gtamprifoc.html

[R30] 函数返回状态码
来源：http://hz.ybcxt.top/gtasqovtzw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gtlwtkhdep.html

[R31] 局部变量
来源：http://hz.zhongyouzk.top/gtzmlrlxqy.html

f() { local x=1; echo "$x"; }
来源：http://hz.cheryme.top/gtuzjbxiha.html

[R32] 参数个数校验
来源：http://hz.c1oappe.top/gtaprtutup.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtbtrzegwv.html

[R33] 捕获错误并提示行号
来源：http://hz.yvedp.cn/gtcdylnhpn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.quarkkingdee.top/gtwwfzhwtx.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gtjkeefwtr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhijiandao.cn/gtylgdcxul.html

[R35] 后台执行并等待
来源：http://hz.9152youxi.cn/gtjanwxowp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj202588.top/gtqbkldtto.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtozmcogpm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fengsongda.top/gtadrqxepk.html

[R37] 把输出赋给变量
来源：http://hz.gogol.net.cn/gtpinvzghf.html

files=$(ls -1)
来源：http://hz.hammf.cn/gtyqfzcnge.html

[R38] 管道串联
来源：http://hz.hongshengwenyu.top/gtgqjxxckz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.vqdsnc.cn/gtolctdotp.html

[R39] 重定向标准输出与错误
来源：http://hz.pengpengdd.cyou/gtfkvbvylq.html

cmd > out.log 2>&1
来源：http://hz.sufxvd.cn/gtafqvsigt.html

[R40] 追加写日志
来源：http://hz.zhiwuduotai.top/gtbdtekwlp.html

echo "log" >> out.log
来源：http://hz.guannengcc.top/gtvnscljlc.html

[R41] 丢弃输出
来源：http://hz.xylfe.cn/gtqrtibqeu.html

cmd >/dev/null 2>&1
来源：http://hz.quarkkingdee.top/gtidtgtdud.html

[R42] 输入重定向
来源：http://hz.chenzaomai.com/gtxrihmqhj.html

wc -l < a.txt
来源：http://hz.andypj.xyz/gtomjvtuct.html

[R43] 按名字查找文件
来源：http://hz.yj20258888.top/gtriclmusp.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtssneebau.html

[R44] 按修改时间查找
来源：http://hz.yuxming.cn/gtmfymmrat.html

find . -mtime -7 -type f
来源：http://hz.316326.xyz/gtaqjxrcin.html

[R45] 批量删除
来源：http://hz.yangfankeji.com/gtstviwqiw.html

find . -name "*.tmp" -delete
来源：http://hz.chenlongwang.top/gttowovecb.html

[R46] 递归替换文件内容
来源：http://hz.jinqigfzy.top/gtjzsjbems.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gtcwpqcpko.html

[R47] sed 单行替换
来源：http://hz.daxiang520.top/gtwdpaeuse.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.bjfxy.top/gtxkmcdpbx.html

[R48] awk 取指定列
来源：http://hz.sxryk.cn/gtblndhxep.html

awk '{print $1, $3}' a.txt
来源：http://hz.xinyue.icu/gtjmbcilhe.html

[R49] awk 带条件
来源：http://hz.jinyuanbaomall.cn/gtaulmtppv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shzxlz.cn/gthrummywf.html

[R50] awk 求和
来源：http://hz.sweek.top/gthylyihwv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnxiangtu.top/gtpqbfklkd.html

[R51] 排序去重取前几
来源：http://hz.shanyushiyangtech.top/gtfagkjofc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tian-w.cn/gtcuvpctfp.html

[R52] 统计行数
来源：http://hz.xingfuxueyuan.xyz/gtfosggmbo.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gtaaetckfl.html

[R53] 查看文件头与实时尾
来源：http://hz.jyoumei.cn/gtkdsmavxt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gtvrsiaebt.html

[R54] 比较两个文件
来源：http://hz.zhongyouzk.top/gtquikmiji.html

diff a.txt b.txt
来源：http://hz.sweek.top/gtaywuxmvd.html

[R55] 压缩与解压
来源：http://hz.guannengcc.top/gtndwjbtsv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigufen.top/gtgphxtsls.html

[R56] 远程拷贝
来源：http://hz.vqdsnc.cn/gtkvwpgfsr.html

scp file user@host:/path/
来源：http://hz.zhoulong.xyz/gtpaemwepm.html

[R57] 远程执行命令
来源：http://hz.tian-w.cn/gttihrgdtr.html

ssh user@host 'uptime'
来源：http://hz.hammf.cn/gtgsyuqzdu.html

[R58] 下载文件
来源：http://hz.pengpengdd.cyou/gtoxjbibxt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cashguo.top/gtralihmvq.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gtbghxqobb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sysykeji.top/gthsxtnlea.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtrngmyori.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jlsjyb.cn/gtncbjpboq.html

[R61] 磁盘占用
来源：http://hz.guowangkeji.top/gtcmeookul.html

df -h;  du -sh *
来源：http://hz.yj20258.top/gtvasaftpw.html

[R62] 找最占空间的文件
来源：http://hz.zhoulong.xyz/gtijmwxhkm.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtnebwslok.html

[R63] 内存与进程
来源：http://hz.hongshengwenyu.top/gtbznmcnnz.html

free -h;  ps aux | grep nginx
来源：http://hz.zhaomingkeji.xyz/gtzrdqbsbj.html

[R64] 结束进程
来源：http://hz.316326.xyz/gtbgpugqco.html

kill -9 $(pgrep -f app.py)
来源：http://hz.iojbl.cn/gtepngfvyy.html

[R65] 查看端口占用
来源：http://hz.yvedp.cn/gtpjqswbwn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.birdmap.top/gtovlsumwj.html

[R66] 定时任务
来源：http://hz.jinqigufen.top/gtcwrjqqzq.html

crontab -e;  crontab -l
来源：http://hz.tanke756.top/gtlqtiycgk.html

[R67] 生成随机十六进制串
来源：http://hz.yonumen.top/gtjuybeyvm.html

openssl rand -hex 16
来源：http://hz.cashguo.top/gttovpenig.html

[R68] 计算文件校验值
来源：http://hz.xylfe.cn/gtudkkkwls.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtdcrivsix.html

[R69] 生成随机密码
来源：http://hz.gogol.net.cn/gtxratyqas.html

head -c 16 /dev/urandom | base64
来源：http://hz.jqgfzy.top/gtrqbcptid.html

[R70] 时间戳与互转
来源：http://hz.316326.xyz/gtucqeqaud.html

date +%s;  date -d @1700000000
来源：http://hz.ywan-chungtsiang.top/gtandvwncs.html

[R71] 日期格式化
来源：http://hz.jyoumei.cn/gthsrdyudn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ybcxt.top/gtreqcxefi.html

[R72] 等待端口就绪
来源：http://hz.zhixingplan.top/gtdlbkmcva.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xuetiantiany.cn/gtxxqiheko.html

[R73] 分割大日志
来源：http://hz.zhijiandao.cn/gtdknuaicy.html

split -l 1000 big.log part_
来源：http://hz.c1oappe.top/gtmshbvfmg.html

[R74] 批量重命名
来源：http://hz.birdmap.top/gttcpeslnt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangtech.top/gtjvlrypcx.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtrizhmigc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnxiangtu.top/gtjmglqpic.html

[R76] 使用临时文件
来源：http://hz.shuidangran.top/gtngzyjpwe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtqglaupxw.html

[R77] 读取用户输入
来源：http://hz.iojbl.cn/gtlnwufrtd.html

read -rp "请输入: " ans
来源：http://hz.cheryme.top/gtpyytywya.html

[R78] 交互式菜单
来源：http://hz.sufxvd.cn/gtjvvxrhwb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gogol.net.cn/gtidusmfkj.html

[R79] 解析命令行选项
来源：http://hz.ydjk.org.cn/gtbujeijhj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gotoacloud.top/gthbpdzocr.html

[R80] 查看脚本执行耗时
来源：http://hz.fzhhl.top/gtzecgcjzj.html

time ./run.sh
来源：http://hz.pycfn.com/gtrkyjiqgh.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfhkazjdx.html

S. C / C++ 专题
来源：http://hz.yanxiufei.cn/gtwnrsyadk.html

================================================================================
来源：http://hz.pycfn.com/gtplrwveiy.html

[S01] C：Hello World
来源：http://hz.tanke756.top/gtqogkuymq.html

#include <stdio.h>
来源：http://hz.jinghuilouyu.cn/gtnckufkfg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zycfv.cn/gtglyjdovc.html

[S02] C：变量与格式化输出
来源：http://hz.sweek.top/gtvuyasssk.html

int a = 10; printf("%d\n", a);
来源：http://hz.feifeiyinyue.top/gtmyutrphk.html

[S03] C：读入整数
来源：http://hz.yueranfly.top/gtbqvfvvkb.html

int x; scanf("%d", &x);
来源：http://hz.316326.xyz/gteobdkhhz.html

[S04] C：字符串复制
来源：http://hz.nanxinkj.top/gtjvmjzlaw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhijiandao.cn/gtevnfixdc.html

[S05] C：字符串长度
来源：http://hz.cheryme.top/gtiwnwnknq.html

strlen(s)
来源：http://hz.tanke756.top/gtticctkbr.html

[S06] C：字符串比较
来源：http://hz.shanyushiyangkeji.top/gtqoitmiuq.html

strcmp(a, b) == 0
来源：http://hz.birdmap.top/gtcgumrcot.html

[S07] C：数组遍历求和
来源：http://hz.sysykeji.top/gtxrknznrg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.52xcode.cn/gtzawhzwlf.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgfzy.top/gtqfkpcqnu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.c1oappe.top/gturopcakf.html

[S09] C：结构体定义与初始化
来源：http://hz.9152youxi.cn/gtxyrhuodf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.wangdashe.top/gtwpirbdzn.html

[S10] C：指针与解引用
来源：http://hz.gzhubu.top/gtbmtlrzqz.html

int *p = &a;  *p = 5;
来源：http://hz.shuidangran.top/gtkepxyrku.html

[S11] C：逐行读文件
来源：http://hz.svipenyu.cn/gtlxaqttwy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sysykeji.top/gtgshwhzgs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yueranfly.top/gtcdccccng.html

fclose(f);
来源：http://hz.mhx1999.top/gtmrvzgrdy.html

[S12] C：写文件
来源：http://hz.zhongyouzk.top/gtutyalgtx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtflesmcqv.html

[S13] C：宏定义
来源：http://hz.zhengqikj.top/gtlcwumswr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhixingplan.top/gtjjnewppq.html

[S14] C：枚举
来源：http://hz.fengsongda.top/gtsekvrwiu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shzxlz.cn/gtemrqybrv.html

[S15] C：类型转换
来源：http://hz.chenjidiqi.icu/gtjtoimwuy.html

(double) a / b
来源：http://hz.zycfv.cn/gtssffoxeb.html

[S16] C：位操作置位
来源：http://hz.nanxuanxn.top/gtyvddkvve.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtwxqspwvf.html

[S17] C：安全拼接字符串
来源：http://hz.shzxlz.cn/gtfsmpgfeq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxuanxn.top/gtsqctkkid.html

[S18] C：命令行参数
来源：http://hz.yangfankeji.com/gtgebmvsoi.html

int main(int argc, char **argv)
来源：http://hz.cashguo.top/gtphjdqpno.html

[S19] C：快速排序
来源：http://hz.xziqi.cn/gtopuawrrj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinyuanbaomall.cn/gtlikkqtbq.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtoehsjllu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtqdkyntzr.html

[S21] C：字符类别判断
来源：http://hz.jyoumei.cn/gtnpimkivd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxinkj.top/gtzsgipokg.html

[S22] C：字符串转数字
来源：http://hz.nanxuanxn.top/gtqsmtjony.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shanyushiyangkeji.top/gtdeekvccy.html

[S23] C：随机数
来源：http://hz.jinghuilouyu.cn/gtdbstcrzl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sufxvd.cn/gtrxuysxri.html

[S24] C：获取本地时间
来源：http://hz.yangfankeji.com/gtlxwkbkvp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hfpthk.cn/gtafkbjrmd.html

[S25] C：内存拷贝
来源：http://hz.xingfuxueyuan.xyz/gtybqnrnsi.html

memcpy(dst, src, n);
来源：http://hz.cashguo.top/gtwormcnwd.html

[S26] C：内存清零
来源：http://hz.dashuyun.cn/gtkquyyfzz.html

memset(a, 0, sizeof a);
来源：http://hz.meibo888.top/gtvrqqtjha.html

[S27] C：定义常量
来源：http://hz.gotoacloud.top/gtlcsiitlk.html

const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtqsmaomzo.html

[S28] C：静态变量
来源：http://hz.yj20258.top/gtgjwsrzdb.html

static int counter = 0;
来源：http://hz.jyoumei.cn/gtxjxdxxce.html

[S29] C：变参函数
来源：http://hz.quarkkingdee.top/gtbyqgvbmx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuetiantiany.cn/gtsmpliblh.html

[S30] C：头文件保护
来源：http://hz.hywenlv.cn/gtvfhwlhfv.html

#ifndef X_H
来源：http://hz.ehwqpu.com/gthwmjtztn.html

#define X_H
来源：http://hz.hnqzz.top/gtzjkowwid.html

#endif
来源：http://hz.jiagoushi.top/gtaclcicnn.html

[S31] C++：Hello World
来源：http://hz.svipenyu.cn/gtjahrcxzm.html

#include <iostream>
来源：http://hz.jinghuilouyu.cn/gtlpcqxdra.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuanzx.com/gtjbekoqpp.html

[S32] C++：字符串
来源：http://hz.jqgufenzy.top/gtgvjtcfyg.html

std::string s = "hi";  s += "!";
来源：http://hz.hnxiangtu.top/gtbjymhmar.html

[S33] C++：vector 增删
来源：http://hz.meibo888.top/gtnqfbxrfu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.havefunace.top/gtevaidtja.html

[S34] C++：遍历 vector
来源：http://hz.jyoumei.cn/gtqtmxyzvs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangkeji.top/gtyvuioogo.html

[S35] C++：map
来源：http://hz.jiagoushi.top/gtmhmeggwr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gttdvmvbaq.html

[S36] C++：unordered_map
来源：http://hz.jinqigfzy.top/gtbaxvcumc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fzhhl.top/gtjfkijdkj.html

[S37] C++：set
来源：http://hz.cucudq.cn/gtwqhkimpo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.0kj1m.cn/gtuufhhwjs.html

[S38] C++：排序
来源：http://hz.xuetiantiany.cn/gtktpgvijf.html

std::sort(v.begin(), v.end());
来源：http://hz.zhijiandao.cn/gtrvbgxkkc.html

[S39] C++：自定义比较器排序
来源：http://hz.kuanghao11.cn/gtqfktsbgb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.havefunace.top/gtzfehbsoe.html

[S40] C++：查找元素
来源：http://hz.zhoulong.xyz/gtshntjgul.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuetiantiany.cn/gtvgvzcsdc.html

[S41] C++：类与构造函数
来源：http://hz.tianlin.xyz/gtymvmmhro.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xziqi.cn/gtdirqjltt.html

[S42] C++：继承与虚函数
来源：http://hz.svipenyu.cn/gtbdjkzygs.html

class B : public Base { public: void f() override {} };
来源：http://hz.shzxlz.cn/gttlwaqwdo.html

[S43] C++：智能指针
来源：http://hz.fengsongda.top/gtjrbntgpn.html

auto p = std::make_unique<int>(5);
来源：http://hz.xinyue.icu/gtenlgivrd.html

[S44] C++：引用传参
来源：http://hz.zhengqikj.top/gtyrfrboqc.html

void inc(int &x) { ++x; }
来源：http://hz.zhoulong.xyz/gthmnlttxs.html

[S45] C++：lambda
来源：http://hz.jyoumei.cn/gtmdgrdyio.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhengqikj.top/gtsmlpjoab.html

[S46] C++：函数模板
来源：http://hz.xuetiantiany.cn/gtwbswoali.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gtgijeqwog.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinyuanbaomall.cn/gtapiehqjd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yuanzhike.top/gtpnpdyxba.html

[S48] C++：逐行读文件
来源：http://hz.xinyue.icu/gtlhuaphxd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.0kj1m.cn/gtlsidsoxu.html

while (std::getline(in, line)) { }
来源：http://hz.yangfankeji.com/gtguvmkaxk.html

[S49] C++：写文件
来源：http://hz.xziqi.cn/gtybexchvv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daria6918.cn/gtpdqnnsmh.html

[S50] C++：格式化数字
来源：http://hz.zhengqikj.top/gtukczubxo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.meibo888.top/gtbxreqegl.html

[S51] C++：显式类型转换
来源：http://hz.gotoacloud.top/gtkzqmofhj.html

static_cast<double>(a) / b
来源：http://hz.hnqzz.top/gtrvgtwyqu.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangtech.top/gtzhcybfme.html

int size() const noexcept { return n_; }
来源：http://hz.wangdashe.top/gtdusglgdx.html

[S53] C++：移动语义
来源：http://hz.yuxming.cn/gtceujwskv.html

std::vector<int> w = std::move(v);
来源：http://hz.c1oappe.top/gtqzbwdwfe.html

[S54] C++：异常处理
来源：http://hz.guowangkeji.top/gttcuairgo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.svipenyu.cn/gtadwtoqwr.html

[S55] C++：结构化绑定
来源：http://hz.jqgfzy.top/gtocdakssu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.smart0.xyz/gtndnmgjty.html

[S56] C++：optional
来源：http://hz.daria6918.cn/gtbebmcvol.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cheryme.top/gtqgbswlja.html

[S57] C++：编译期常量
来源：http://hz.pengpengdd.cyou/gtbposzpix.html

constexpr int N = 10;
来源：http://hz.jinqigufen.top/gtvvcirgnw.html

[S58] C++：命名空间
来源：http://hz.xylfe.cn/gtcfhkzucy.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangtech.top/gtjmfwjlbm.html

[S59] C++：静态断言
来源：http://hz.0kj1m.cn/gtvihqskpv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.havefunace.top/gtgcztadtv.html

[S60] C++：遍历并删除元素
来源：http://hz.wangshuangyany.cn/gtbdcgafog.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxinkj.top/gtbvpycfva.html

================================================================================
来源：http://hz.jinqigfzy.top/gtprkysftg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yangfankeji.com/gtanordrdk.html

================================================================================
来源：http://hz.hysaishi.cn/gtzmyrojil.html


<!-- 参考信息 -->