代发 wailian999

R. Bash 专题
来源：http://hz.wangshuangyany.cn/gtruvfsqmi.html

================================================================================
来源：http://hz.yj20258888.top/gtukmigrzu.html

[R01] shebang 与严格模式
来源：http://hz.yongpay.top/gtldwtguzf.html

#!/usr/bin/env bash
来源：http://hz.tanke756.top/gtswhiofch.html

set -euo pipefail
来源：http://hz.shanyushiyangtech.top/gtttblxvdf.html

[R02] 变量赋值与使用
来源：http://hz.xuanzx.com/gtstqxzvip.html

name="Tom"; echo "$name"
来源：http://hz.andypj.xyz/gtpvkuhbcf.html

[R03] 只读变量
来源：http://hz.jqgufenzy.top/gtcvmygpet.html

readonly PI=3.14
来源：http://hz.zhengqikj.top/gtttzqmmnf.html

[R04] 位置参数
来源：http://hz.daria6918.cn/gtoskeiksd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cdnleiting.top/gtaixzbrrb.html

[R05] 参数默认值
来源：http://hz.xylfe.cn/gtkftogyco.html

name="${1:-default}"
来源：http://hz.birdmap.top/gtetmruqyq.html

[R06] 判断命令是否存在
来源：http://hz.andypj.xyz/gtzpxithdg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aizwys.cn/gthrqlzkwg.html

[R07] if 判断文件
来源：http://hz.fzhhl.top/gtcglcbkae.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jiagoushi.top/gtlrqyywbu.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gtawdjaxid.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yangfankeji.com/gtfysbtjqw.html

[R09] 字符串比较
来源：http://hz.fzhhl.top/gtmtlsyjst.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ppjwa.cn/gtzdgcvjkr.html

[R10] 正则匹配
来源：http://hz.yonumen.top/gtbrvczmvp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuxming.cn/gtbrdhlscq.html

[R11] case 多分支
来源：http://hz.cashguo.top/gtnysevrao.html

case "$1" in
来源：http://hz.sxryk.cn/gtvpdjwrhz.html

start) echo "启动" ;;
来源：http://hz.cdnleiting.top/gtwxtpupgg.html

stop)  echo "停止" ;;
来源：http://hz.wangshuangyany.cn/gthzmnmequ.html

*)     echo "未知命令" ;;
来源：http://hz.jinyuanbaomall.cn/gtwhgvqazy.html

esac
来源：http://hz.zycfv.cn/gtwcgayhkx.html

[R12] for 遍历文件
来源：http://hz.yangfankeji.com/gtbpjsgiyz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.316326.xyz/gtnkgzohyo.html

[R13] for 计数循环
来源：http://hz.daxiang520.top/gtwfmzhwgu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tianlin.xyz/gtkjtzisua.html

[R14] C 风格 for
来源：http://hz.quarkkingdee.top/gtdlbvmllc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sysykeji.top/gtcetbhdnp.html

[R15] while 逐行读文件
来源：http://hz.0kj1m.cn/gtrqpdkhsi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yanxiufei.cn/gthkjchnin.html

[R16] until 等待条件
来源：http://hz.sxryk.cn/gtupnyzqcc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hysaishi.cn/gtvszgwgxi.html

[R17] 数组定义与取值
来源：http://hz.hammf.cn/gtseptmnhn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgufenzy.top/gtkbpdzjsz.html

[R18] 遍历数组
来源：http://hz.dashuyun.cn/gtnclgclvm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gtblbschuo.html

[R19] 数组长度
来源：http://hz.jiagoushi.top/gtyjzowqfb.html

echo "${#arr[@]}"
来源：http://hz.wangshuangyany.cn/gtkaooeecu.html

[R20] 关联数组（字典）
来源：http://hz.zhoulong.xyz/gtuagjrppb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.mhx1999.top/gtgwskhkpq.html

[R21] 字符串长度
来源：http://hz.daria6918.cn/gtwkdktvte.html

echo "${#s}"
来源：http://hz.zycfv.cn/gtouqvmkvu.html

[R22] 截取子串
来源：http://hz.zhoulong.xyz/gtuffwhwtf.html

echo "${s:0:5}"
来源：http://hz.wangshuangyany.cn/gtyzzkuqmy.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtzvomulxd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daria6918.cn/gtxgwrjnxg.html

[R24] 大小写转换
来源：http://hz.xuetiantiany.cn/gtvyenwudo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangkeji.top/gtbdslcjgi.html

[R25] 去后缀 / 去前缀
来源：http://hz.xingfuxueyuan.xyz/gtuwmivotd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.iojbl.cn/gtednytpum.html

[R26] 命令替换
来源：http://hz.hywenlv.cn/gtzaejzjlk.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgfzy.top/gtxfhlbccn.html

[R27] 算术展开
来源：http://hz.ybcxt.top/gtelybmtni.html

echo $((1 + 2 * 3))
来源：http://hz.zycfv.cn/gtpxttquzw.html

[R28] 浮点运算
来源：http://hz.gotoacloud.top/gtnudjbtou.html

echo "scale=2; 10/3" | bc
来源：http://hz.cqqwz.cn/gtvfecbrrv.html

[R29] 定义函数
来源：http://hz.jinghuilouyu.cn/gtxrnyltak.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yangfankeji.com/gtugaqheqo.html

[R30] 函数返回状态码
来源：http://hz.chenlongwang.top/gtakagcdbe.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sweek.top/gtjcrbmfzq.html

[R31] 局部变量
来源：http://hz.c1oappe.top/gtiiqxeuqw.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtzjbnzvyg.html

[R32] 参数个数校验
来源：http://hz.yongpay.top/gtjywigwgk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sysykeji.top/gtcpiouoyy.html

[R33] 捕获错误并提示行号
来源：http://hz.wangshuangyany.cn/gtjpbyzihu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtqfqpisru.html

[R34] 退出时清理
来源：http://hz.wangshuangyany.cn/gtnhoviavb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtljkzvcqa.html

[R35] 后台执行并等待
来源：http://hz.redwolf501.top/gtfamuilnz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenlongwang.top/gtnzhthvwf.html

[R36] 并发执行多个任务
来源：http://hz.nanxinkj.top/gtxzkgswto.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jiagoushi.top/gtotfbwxli.html

[R37] 把输出赋给变量
来源：http://hz.zycfv.cn/gttsmnanqf.html

files=$(ls -1)
来源：http://hz.gaohongyu789.top/gtlgodqazu.html

[R38] 管道串联
来源：http://hz.xuetiantiany.cn/gtcqiyhfpm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daria6918.cn/gtpfgvddab.html

[R39] 重定向标准输出与错误
来源：http://hz.cashguo.top/gtnqjqlxjg.html

cmd > out.log 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtmkbhoisl.html

[R40] 追加写日志
来源：http://hz.daxiang520.top/gtemdxwapt.html

echo "log" >> out.log
来源：http://hz.wangshuangyany.cn/gtdzgjxmgc.html

[R41] 丢弃输出
来源：http://hz.cashguo.top/gthlftfcny.html

cmd >/dev/null 2>&1
来源：http://hz.yuanzhike.top/gthgrfbkkk.html

[R42] 输入重定向
来源：http://hz.aizwys.cn/gtmaqcadwb.html

wc -l < a.txt
来源：http://hz.hnxiangtu.top/gtogoskmwg.html

[R43] 按名字查找文件
来源：http://hz.gzhubu.top/gtkbdnzunz.html

find . -name "*.log" -type f
来源：http://hz.gogol.net.cn/gtkaxererq.html

[R44] 按修改时间查找
来源：http://hz.iojbl.cn/gtpqmcrdef.html

find . -mtime -7 -type f
来源：http://hz.0kj1m.cn/gtmpptgzby.html

[R45] 批量删除
来源：http://hz.yuxming.cn/gtigdapiyy.html

find . -name "*.tmp" -delete
来源：http://hz.sweek.top/gtldrgpxje.html

[R46] 递归替换文件内容
来源：http://hz.bjfxy.top/gtlnkxdtnx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhixingplan.top/gtofcgwlwa.html

[R47] sed 单行替换
来源：http://hz.0kj1m.cn/gtsscqgjcd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hysaishi.cn/gtxbdmcrdg.html

[R48] awk 取指定列
来源：http://hz.redwolf501.top/gtbjieundt.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenlongwang.top/gtikzsowys.html

[R49] awk 带条件
来源：http://hz.zhongyouzk.top/gtydrmylqa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tanke756.top/gtbvbxfirj.html

[R50] awk 求和
来源：http://hz.pycfn.com/gtdognkwwy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aizwys.cn/gtbxfurbvz.html

[R51] 排序去重取前几
来源：http://hz.cucudq.cn/gtvhtadjae.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhijiandao.cn/gtbmmbpwmm.html

[R52] 统计行数
来源：http://hz.vqdsnc.cn/gtbtxgshdc.html

wc -l a.txt
来源：http://hz.kuanghao11.cn/gtkaxlqzoh.html

[R53] 查看文件头与实时尾
来源：http://hz.xylfe.cn/gtblcsaocw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cucudq.cn/gtpcokicei.html

[R54] 比较两个文件
来源：http://hz.yuanzhike.top/gtkyjtrpfb.html

diff a.txt b.txt
来源：http://hz.gaohongyu789.top/gtkdnpwann.html

[R55] 压缩与解压
来源：http://hz.daxiang520.top/gtzgqvommi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xziqi.cn/gtneotcvpt.html

[R56] 远程拷贝
来源：http://hz.xuetiantiany.cn/gtqlgkvncc.html

scp file user@host:/path/
来源：http://hz.0kj1m.cn/gtlveircxz.html

[R57] 远程执行命令
来源：http://hz.xingfuxueyuan.xyz/gtnokbulld.html

ssh user@host 'uptime'
来源：http://hz.ydzc1.top/gtcqcalcip.html

[R58] 下载文件
来源：http://hz.zdqjudy.top/gthcopnxlf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hysaishi.cn/gtepxhcwwh.html

[R59] 发 POST JSON
来源：http://hz.chenjidiqi.icu/gtpkyvmffh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tian-w.cn/gtpabgduvj.html

[R60] 只看 HTTP 状态码
来源：http://hz.aizwys.cn/gtaqwedfrq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hongshengwenyu.top/gtsxpjlupy.html

[R61] 磁盘占用
来源：http://hz.yuxming.cn/gtxakuwqtc.html

df -h;  du -sh *
来源：http://hz.guannengcc.top/gtfsndjxhx.html

[R62] 找最占空间的文件
来源：http://hz.yj20258.top/gttsuquvqj.html

du -ah . | sort -rh | head -10
来源：http://hz.52xcode.cn/gtdhdsgick.html

[R63] 内存与进程
来源：http://hz.ydjk.org.cn/gtryjhfzga.html

free -h;  ps aux | grep nginx
来源：http://hz.feifeiyinyue.top/gtytvtzzib.html

[R64] 结束进程
来源：http://hz.ybcxt.top/gtjqpvgxyk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.smart0.xyz/gtqdxqqmdq.html

[R65] 查看端口占用
来源：http://hz.ywan-chungtsiang.top/gtjaspflip.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daria6918.cn/gtvlnbaxhl.html

[R66] 定时任务
来源：http://hz.xinyue.icu/gtzcecyyhg.html

crontab -e;  crontab -l
来源：http://hz.pengpengdd.cyou/gtldbakwqy.html

[R67] 生成随机十六进制串
来源：http://hz.mhx1999.top/gtwojbrvum.html

openssl rand -hex 16
来源：http://hz.kuanghao11.cn/gtrqkbifkr.html

[R68] 计算文件校验值
来源：http://hz.sysykeji.top/gtdstcjzdf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tanke756.top/gtobsspdas.html

[R69] 生成随机密码
来源：http://hz.cheryme.top/gtvyzwjvsy.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhengqikj.top/gtxtukbtrt.html

[R70] 时间戳与互转
来源：http://hz.xziqi.cn/gtxnpjuwun.html

date +%s;  date -d @1700000000
来源：http://hz.shangyingyoupin.top/gtpxwcxozj.html

[R71] 日期格式化
来源：http://hz.chenlongwang.top/gtcvxidznc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.iojbl.cn/gtuxvxqlsw.html

[R72] 等待端口就绪
来源：http://hz.bjfxy.top/gtncajcvaq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.316326.xyz/gtkurbdifs.html

[R73] 分割大日志
来源：http://hz.shangyingyoupin.top/gtmuyxagoy.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangtech.top/gtoecwyvzz.html

[R74] 批量重命名
来源：http://hz.52xcode.cn/gtfxmkyvvg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nanxinkj.top/gtcdomrvgj.html

[R75] 导出环境变量
来源：http://hz.pycfn.com/gtijfwoprm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.guannengcc.top/gteykqrwdi.html

[R76] 使用临时文件
来源：http://hz.hnqzz.top/gtuttnizya.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtwyveqnst.html

[R77] 读取用户输入
来源：http://hz.shanyushiyangkeji.top/gthwsejvox.html

read -rp "请输入: " ans
来源：http://hz.jinqigfzy.top/gtdhkjqnge.html

[R78] 交互式菜单
来源：http://hz.ywan-chungtsiang.top/gtkiekeeiw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xuanzx.com/gttwhdxofx.html

[R79] 解析命令行选项
来源：http://hz.jinqigufen.top/gtgybeslgz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.wangdashe.top/gtwipgtwkw.html

[R80] 查看脚本执行耗时
来源：http://hz.jyoumei.cn/gtspirihvr.html

time ./run.sh
来源：http://hz.ywan-chungtsiang.top/gtmobusjas.html

================================================================================
来源：http://hz.jinqigfzy.top/gtzevwiwrf.html

S. C / C++ 专题
来源：http://hz.shzxlz.cn/gtmrojttow.html

================================================================================
来源：http://hz.ehwqpu.com/gtuiscnway.html

[S01] C：Hello World
来源：http://hz.svipenyu.cn/gtfmhllwsr.html

#include <stdio.h>
来源：http://hz.cheryme.top/gtwrkafvhs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.9152youxi.cn/gtluastcli.html

[S02] C：变量与格式化输出
来源：http://hz.ivvv.top/gtnltkrgbx.html

int a = 10; printf("%d\n", a);
来源：http://hz.jyoumei.cn/gtxgacibvt.html

[S03] C：读入整数
来源：http://hz.guowangkeji.top/gtghoonewy.html

int x; scanf("%d", &x);
来源：http://hz.ydzc1.top/gtyrqgkohg.html

[S04] C：字符串复制
来源：http://hz.zhengqikj.top/gtqfqicsiv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuxming.cn/gtticnowdl.html

[S05] C：字符串长度
来源：http://hz.chenlongwang.top/gtfksuiswr.html

strlen(s)
来源：http://hz.zhixingplan.top/gtarnaphfv.html

[S06] C：字符串比较
来源：http://hz.sxryk.cn/gtkyfdjhdd.html

strcmp(a, b) == 0
来源：http://hz.tanke756.top/gtpbglhswi.html

[S07] C：数组遍历求和
来源：http://hz.jinyuanbaomall.cn/gtkxvxhztl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gtncxhuocj.html

[S08] C：动态内存分配与释放
来源：http://hz.iojbl.cn/gtjfekmogb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.svipenyu.cn/gtqiwakaeg.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgufenzy.top/gthzrtpaww.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuetiantiany.cn/gtahfxjcgy.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gtxwyrzgrh.html

int *p = &a;  *p = 5;
来源：http://hz.quarkkingdee.top/gthyonynba.html

[S11] C：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtmwwlbxjr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xylfe.cn/gttvzbebvv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.andypj.xyz/gtnjfqfulr.html

fclose(f);
来源：http://hz.yanxiufei.cn/gtalmwppnt.html

[S12] C：写文件
来源：http://hz.0kj1m.cn/gtqafqoeau.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinghuilouyu.cn/gtyxcnurbi.html

[S13] C：宏定义
来源：http://hz.xylfe.cn/gtmftyqsmk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinyuanbaomall.cn/gtjmtuhdzo.html

[S14] C：枚举
来源：http://hz.daxiang520.top/gtbbrbiqib.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fengsongda.top/gthcfymomh.html

[S15] C：类型转换
来源：http://hz.yuanzhike.top/gtmskglwwb.html

(double) a / b
来源：http://hz.jqgufenzy.top/gtrvbclxam.html

[S16] C：位操作置位
来源：http://hz.birdmap.top/gtotdvkehe.html

x |= (1 << 3);
来源：http://hz.aibaodan.cn/gtzfkggqwp.html

[S17] C：安全拼接字符串
来源：http://hz.xuetiantiany.cn/gtazpflnow.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cashguo.top/gticgyffoc.html

[S18] C：命令行参数
来源：http://hz.gogol.net.cn/gtzzlystsi.html

int main(int argc, char **argv)
来源：http://hz.yj202588.top/gtsrthqoqu.html

[S19] C：快速排序
来源：http://hz.zhongyouzk.top/gtwamhudqc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtqvauvvrl.html

[S20] C：二分查找
来源：http://hz.shangyingyoupin.top/gtjzjrofzd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gtpreedrmp.html

[S21] C：字符类别判断
来源：http://hz.c1oappe.top/gthdmhgtow.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhengqikj.top/gtscoyrekr.html

[S22] C：字符串转数字
来源：http://hz.sweek.top/gtsxcgmakh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.quarkkingdee.top/gtqkczhmoh.html

[S23] C：随机数
来源：http://hz.shanyushiyangkeji.top/gtwzyeaznv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hongshengwenyu.top/gtqgmftfhi.html

[S24] C：获取本地时间
来源：http://hz.redwolf501.top/gtazimqsgv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cashguo.top/gtafusrvqj.html

[S25] C：内存拷贝
来源：http://hz.bjfxy.top/gtxmccmfdg.html

memcpy(dst, src, n);
来源：http://hz.nanxinkj.top/gtkvmltzqy.html

[S26] C：内存清零
来源：http://hz.daria6918.cn/gtwszmpnqy.html

memset(a, 0, sizeof a);
来源：http://hz.jinyuanbaomall.cn/gtqhrfublo.html

[S27] C：定义常量
来源：http://hz.haohaochexian.top/gtagqoerns.html

const double PI = 3.14159;
来源：http://hz.dianchejie.cn/gtgnlakssg.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtwykttitu.html

static int counter = 0;
来源：http://hz.jqgufenzy.top/gtgtgbrlvx.html

[S29] C：变参函数
来源：http://hz.jianghu66.top/gtzkkgubjt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.feifeiyinyue.top/gtgkqxkiez.html

[S30] C：头文件保护
来源：http://hz.gaohongyu789.top/gtowpwtidc.html

#ifndef X_H
来源：http://hz.hongshengwenyu.top/gtutrzjyoh.html

#define X_H
来源：http://hz.hongshengwenyu.top/gtcertjfhk.html

#endif
来源：http://hz.hnxiangtu.top/gtxfzvqeua.html

[S31] C++：Hello World
来源：http://hz.hywenlv.cn/gtishmdnsj.html

#include <iostream>
来源：http://hz.yanxiufei.cn/gtotdkxolj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jianghu66.top/gtxjwgbbio.html

[S32] C++：字符串
来源：http://hz.smart0.xyz/gtlqsghnot.html

std::string s = "hi";  s += "!";
来源：http://hz.cucudq.cn/gtumrybxym.html

[S33] C++：vector 增删
来源：http://hz.aibaodan.cn/gtkeepjdjn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hysaishi.cn/gtgmbviszh.html

[S34] C++：遍历 vector
来源：http://hz.andypj.xyz/gtuvginkux.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cashguo.top/gtupypovgm.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtpndmqoxt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gtuzugsxqa.html

[S36] C++：unordered_map
来源：http://hz.sysykeji.top/gtezgbkzff.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gtfgesduhd.html

[S37] C++：set
来源：http://hz.kuanghao11.cn/gtjzthaujg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aizwys.cn/gtdavqovgi.html

[S38] C++：排序
来源：http://hz.tianlin.xyz/gtmnlzorxp.html

std::sort(v.begin(), v.end());
来源：http://hz.meibo888.top/gtfmvurdxw.html

[S39] C++：自定义比较器排序
来源：http://hz.fengsongda.top/gthpenxtyx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tianlin.xyz/gtebpgbozh.html

[S40] C++：查找元素
来源：http://hz.zhaomingkeji.xyz/gtodkedany.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigfzy.top/gtlyvmplwy.html

[S41] C++：类与构造函数
来源：http://hz.zhongyouzk.top/gtgvhpigwv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenlongwang.top/gtfxfzzolo.html

[S42] C++：继承与虚函数
来源：http://hz.jlsjyb.cn/gtkjtbqlct.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenjidiqi.icu/gtgdgulvdm.html

[S43] C++：智能指针
来源：http://hz.jinghuilouyu.cn/gtxyuwtouy.html

auto p = std::make_unique<int>(5);
来源：http://hz.gaohongyu789.top/gtzdnpqioi.html

[S44] C++：引用传参
来源：http://hz.andypj.xyz/gtmexyykls.html

void inc(int &x) { ++x; }
来源：http://hz.haohaochexian.top/gtejcvloxz.html

[S45] C++：lambda
来源：http://hz.shzxlz.cn/gtvhvkzkdt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.pycfn.com/gtelcjbpeb.html

[S46] C++：函数模板
来源：http://hz.sysykeji.top/gtkoxlpyse.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.andypj.xyz/gtcbuqkpwy.html

[S47] C++：结构化绑定遍历
来源：http://hz.9152youxi.cn/gtvzrykath.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nanxinkj.top/gtuykacpps.html

[S48] C++：逐行读文件
来源：http://hz.meibo888.top/gtxhbpddho.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinghuilouyu.cn/gtlhxzrgka.html

while (std::getline(in, line)) { }
来源：http://hz.gaohongyu789.top/gtqwuoaska.html

[S49] C++：写文件
来源：http://hz.ivvv.top/gtfatuwtyr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hysaishi.cn/gtugrmnlzn.html

[S50] C++：格式化数字
来源：http://hz.birdmap.top/gteuyngeqi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yanxiufei.cn/gttgikltay.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtjfiqxkio.html

static_cast<double>(a) / b
来源：http://hz.ydzc1.top/gtmcnrbtzy.html

[S52] C++：const 与 noexcept
来源：http://hz.zhongyouzk.top/gtwbqwwqiv.html

int size() const noexcept { return n_; }
来源：http://hz.hywenlv.cn/gtntjhfnjr.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gttvhdbakb.html

std::vector<int> w = std::move(v);
来源：http://hz.zhongyouzk.top/gtdtnnktlh.html

[S54] C++：异常处理
来源：http://hz.ppjwa.cn/gtqghqliaq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yanxiufei.cn/gtpektahof.html

[S55] C++：结构化绑定
来源：http://hz.ywan-chungtsiang.top/gtjzxgxemz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.bjfxy.top/gtgpnreray.html

[S56] C++：optional
来源：http://hz.jqgufenzy.top/gtmtdikykm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.52xcode.cn/gthajnhiuk.html

[S57] C++：编译期常量
来源：http://hz.feifeiyinyue.top/gtoyidfynl.html

constexpr int N = 10;
来源：http://hz.shanyushiyangtech.top/gtlcpubooq.html

[S58] C++：命名空间
来源：http://hz.shuidangran.top/gtyknuhvpx.html

namespace ns { int f() { return 1; } }
来源：http://hz.gaohongyu789.top/gtuspyagze.html

[S59] C++：静态断言
来源：http://hz.sysykeji.top/gtjvuyiwdk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cheryme.top/gteqaleecd.html

[S60] C++：遍历并删除元素
来源：http://hz.aizwys.cn/gtweyujwoc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtocugwhdn.html

================================================================================
来源：http://hz.yueranfly.top/gtdrflmlbb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hnqzz.top/gthomwvcvu.html

================================================================================
来源：http://hz.tianlin.xyz/gtsmsdxeec.html


<!-- 参考信息 -->