代发 wailian999

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gtphmovhmo.html

SELECT TRIM(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtbtitpitr.html

[Q85] 数值取整
来源：http://hz.hongshengwenyu.top/gtexmqybaw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aizwys.cn/gtrewldmbb.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtbfuofava.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cdnleiting.top/gtqjwsnuqh.html

[Q87] JSON 字段做条件
来源：http://hz.yuxming.cn/gtiwcbfvft.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.iojbl.cn/gtjwsnwiin.html

[Q88] 行转列（条件聚合）
来源：http://hz.hysaishi.cn/gtvxileywd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sweek.top/gtfocuzdqb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.vqdsnc.cn/gtxgbgekcc.html

[Q89] 判断表是否存在
来源：http://hz.shzxlz.cn/gtmuhhmapk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.andypj.xyz/gtfobnaxnv.html

[Q90] 生成序号列
来源：http://hz.xziqi.cn/gtjoxadtuz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pengpengdd.cyou/gtglzteoen.html

================================================================================
来源：http://hz.zhengqikj.top/gtxvsfuxnh.html

R. Bash 专题
来源：http://hz.zhengqikj.top/gttifeatfp.html

================================================================================
来源：http://hz.fzhhl.top/gtjmrdgphj.html

[R01] shebang 与严格模式
来源：http://hz.guannengcc.top/gtdclpaqbf.html

#!/usr/bin/env bash
来源：http://hz.nwbrower.top/gtnsxzbeja.html

set -euo pipefail
来源：http://hz.fengsongda.top/gtfhbcclvn.html

[R02] 变量赋值与使用
来源：http://hz.chenzaomai.com/gtaauuvcpc.html

name="Tom"; echo "$name"
来源：http://hz.shuidangran.top/gtwwjpmqob.html

[R03] 只读变量
来源：http://hz.nanxuanxn.top/gtjkghmcob.html

readonly PI=3.14
来源：http://hz.shangyingyoupin.top/gtibwxrtuw.html

[R04] 位置参数
来源：http://hz.hywenlv.cn/gtnztjofoi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinyuanbaomall.cn/gtgwnfzcfh.html

[R05] 参数默认值
来源：http://hz.52xcode.cn/gtcgnihivt.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gtuhxhrmth.html

[R06] 判断命令是否存在
来源：http://hz.zhixingplan.top/gtclqznqgf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hfpthk.cn/gtrntdrcdy.html

[R07] if 判断文件
来源：http://hz.sxryk.cn/gtcdqgctzr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinghuilouyu.cn/gtemhhnokr.html

[R08] 数值比较
来源：http://hz.snrcjt.cn/gtyflbodtg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.bjfxy.top/gtouyzqwsl.html

[R09] 字符串比较
来源：http://hz.quarkkingdee.top/gtmyqymwih.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.guowangkeji.top/gtcpoxrnea.html

[R10] 正则匹配
来源：http://hz.c1oappe.top/gtsexpnlvr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tian-w.cn/gtrhpnoqhs.html

[R11] case 多分支
来源：http://hz.feifeiyinyue.top/gtbmsmeayc.html

case "$1" in
来源：http://hz.chenjidiqi.icu/gtmhpngxgo.html

start) echo "启动" ;;
来源：http://hz.daxiang520.top/gtgxvhlzok.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gtsmkwbjgn.html

*)     echo "未知命令" ;;
来源：http://hz.xinyue.icu/gttepputib.html

esac
来源：http://hz.52xcode.cn/gttvzefnli.html

[R12] for 遍历文件
来源：http://hz.nwbrower.top/gtwjaoyzzt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yongpay.top/gtacceytaq.html

[R13] for 计数循环
来源：http://hz.jyoumei.cn/gtkyltprra.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtoiflmzlv.html

[R14] C 风格 for
来源：http://hz.gotoacloud.top/gthzyonopr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258888.top/gtsxnzxvbh.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gtpmcuihnx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sweek.top/gtzvecawti.html

[R16] until 等待条件
来源：http://hz.nanxinkj.top/gtrhekchzr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhengqikj.top/gtaxrgypmr.html

[R17] 数组定义与取值
来源：http://hz.nwbrower.top/gtlrgjrket.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtdylwlzlv.html

[R18] 遍历数组
来源：http://hz.ydzc1.top/gtlzvesnkz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhiwuduotai.top/gtgrlrgtui.html

[R19] 数组长度
来源：http://hz.hnxiangtu.top/gttvtdbwkp.html

echo "${#arr[@]}"
来源：http://hz.52xcode.cn/gtcbvlwvax.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtmxvylfuh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.redwolf501.top/gtxgvdlkik.html

[R21] 字符串长度
来源：http://hz.pycfn.com/gtvpahrmor.html

echo "${#s}"
来源：http://hz.tanke756.top/gtqbdnvdpk.html

[R22] 截取子串
来源：http://hz.c1oappe.top/gtgrpjhbxp.html

echo "${s:0:5}"
来源：http://hz.smart0.xyz/gtxvtzjzfe.html

[R23] 字符串替换
来源：http://hz.pengpengdd.cyou/gttolgmpgz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tanke756.top/gtwsjhesnw.html

[R24] 大小写转换
来源：http://hz.tianlin.xyz/gtoamvzhnk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gzhubu.top/gtfakuwdxz.html

[R25] 去后缀 / 去前缀
来源：http://hz.ppjwa.cn/gtismnhqdh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fzhhl.top/gtytvmcwbj.html

[R26] 命令替换
来源：http://hz.yueranfly.top/gtfetgdrfl.html

now=$(date +%F); echo "$now"
来源：http://hz.chenzaomai.com/gtullfpyut.html

[R27] 算术展开
来源：http://hz.jinqigfzy.top/gtcwrxawpr.html

echo $((1 + 2 * 3))
来源：http://hz.yanxiufei.cn/gtidrzmzaw.html

[R28] 浮点运算
来源：http://hz.hnqzz.top/gtxuuodckb.html

echo "scale=2; 10/3" | bc
来源：http://hz.316326.xyz/gtwejgjzzj.html

[R29] 定义函数
来源：http://hz.pycfn.com/gttwocelvu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenjidiqi.icu/gtkwaoeent.html

[R30] 函数返回状态码
来源：http://hz.jqgufenzy.top/gtudadjwtb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yueranfly.top/gturmljpgi.html

[R31] 局部变量
来源：http://hz.jinqigfzy.top/gtxtxuadcn.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuxming.cn/gtybengbpg.html

[R32] 参数个数校验
来源：http://hz.hammf.cn/gthdaeoiyz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sxryk.cn/gthwgdoesr.html

[R33] 捕获错误并提示行号
来源：http://hz.yongpay.top/gtmwpuphrz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pengpengdd.cyou/gtlpxoluji.html

[R34] 退出时清理
来源：http://hz.svipenyu.cn/gtuhiyfliu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtrhtihvtc.html

[R35] 后台执行并等待
来源：http://hz.ydjk.org.cn/gtomyimrfr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sufxvd.cn/gtylchmpje.html

[R36] 并发执行多个任务
来源：http://hz.zhengqikj.top/gtfzjhvpov.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sysykeji.top/gtlenglpeh.html

[R37] 把输出赋给变量
来源：http://hz.zdqjudy.top/gtldjntbmq.html

files=$(ls -1)
来源：http://hz.xingfuxueyuan.xyz/gteopuaxei.html

[R38] 管道串联
来源：http://hz.shangyingyoupin.top/gtaqszkzzm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cqqwz.cn/gtmmuucjpn.html

[R39] 重定向标准输出与错误
来源：http://hz.meibo888.top/gtzrasyvap.html

cmd > out.log 2>&1
来源：http://hz.quarkkingdee.top/gtfnabassy.html

[R40] 追加写日志
来源：http://hz.aibaodan.cn/gtcpghlbjy.html

echo "log" >> out.log
来源：http://hz.sufxvd.cn/gttzqvdczs.html

[R41] 丢弃输出
来源：http://hz.52xcode.cn/gtfrszzqyn.html

cmd >/dev/null 2>&1
来源：http://hz.ydzc1.top/gtfixzqegz.html

[R42] 输入重定向
来源：http://hz.zhiwuduotai.top/gtdwgonexm.html

wc -l < a.txt
来源：http://hz.yvedp.cn/gtcaahvmjn.html

[R43] 按名字查找文件
来源：http://hz.ywan-chungtsiang.top/gtwgaclxlx.html

find . -name "*.log" -type f
来源：http://hz.hfpthk.cn/gtmimxdhko.html

[R44] 按修改时间查找
来源：http://hz.yj20258888.top/gtofmnbuua.html

find . -mtime -7 -type f
来源：http://hz.ehwqpu.com/gtfbgdmnqr.html

[R45] 批量删除
来源：http://hz.redwolf501.top/gtarmgkikn.html

find . -name "*.tmp" -delete
来源：http://hz.nwbrower.top/gtwrmtshtj.html

[R46] 递归替换文件内容
来源：http://hz.zhengqikj.top/gtohobrzst.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.havefunace.top/gtxlwmvvhd.html

[R47] sed 单行替换
来源：http://hz.hnqzz.top/gtwbqfqyrx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydjk.org.cn/gtsbjllway.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gtuivcpqrv.html

awk '{print $1, $3}' a.txt
来源：http://hz.birdmap.top/gttdwhwsbt.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtyvhtiscc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.svipenyu.cn/gtalimbdrp.html

[R50] awk 求和
来源：http://hz.hammf.cn/gthxezspxn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.feifeiyinyue.top/gtyakvdvxw.html

[R51] 排序去重取前几
来源：http://hz.zhiwuduotai.top/gtozueeuzz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhijiandao.cn/gtsrlvgmjw.html

[R52] 统计行数
来源：http://hz.wangshuangyany.cn/gtvzouooqn.html

wc -l a.txt
来源：http://hz.yj202588.top/gtogvkedmr.html

[R53] 查看文件头与实时尾
来源：http://hz.pycfn.com/gtcxdjbeqk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.iojbl.cn/gtisouyunq.html

[R54] 比较两个文件
来源：http://hz.316326.xyz/gtkekukrqe.html

diff a.txt b.txt
来源：http://hz.gaohongyu789.top/gtjvxrljji.html

[R55] 压缩与解压
来源：http://hz.pycfn.com/gtiimploec.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xingfuxueyuan.xyz/gtlsechtjd.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtizfvzhfy.html

scp file user@host:/path/
来源：http://hz.zdqjudy.top/gtgmbctnce.html

[R57] 远程执行命令
来源：http://hz.xylfe.cn/gtlddjtera.html

ssh user@host 'uptime'
来源：http://hz.shangyingyoupin.top/gtjhsduroy.html

[R58] 下载文件
来源：http://hz.zycfv.cn/gtrqfapeiy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.smart0.xyz/gtxanciscf.html

[R59] 发 POST JSON
来源：http://hz.yj20258888.top/gtyvinxtbb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.svipenyu.cn/gtixoflxfl.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtbzxgdwtz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jlsjyb.cn/gtycgqfeik.html

[R61] 磁盘占用
来源：http://hz.gaohongyu789.top/gthmllpzbi.html

df -h;  du -sh *
来源：http://hz.dianchejie.cn/gtsgkqrhdj.html

[R62] 找最占空间的文件
来源：http://hz.xuanzx.com/gtebbajqit.html

du -ah . | sort -rh | head -10
来源：http://hz.havefunace.top/gtgstaqoox.html

[R63] 内存与进程
来源：http://hz.meibo888.top/gtxsrxwods.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258.top/gtnekrpwqb.html

[R64] 结束进程
来源：http://hz.zhengqikj.top/gtppmseemb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sxryk.cn/gtbtjoyhpw.html

[R65] 查看端口占用
来源：http://hz.kuanghao11.cn/gtehoeqaej.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgufenzy.top/gthuunyeok.html

[R66] 定时任务
来源：http://hz.gzhubu.top/gtysbfzqig.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangtech.top/gttvsfffro.html

[R67] 生成随机十六进制串
来源：http://hz.zycfv.cn/gtlsnwpmpb.html

openssl rand -hex 16
来源：http://hz.tian-w.cn/gtuhvttvzt.html

[R68] 计算文件校验值
来源：http://hz.vqdsnc.cn/gtxebejcbr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ehwqpu.com/gtzrdyyhjn.html

[R69] 生成随机密码
来源：http://hz.fzhhl.top/gtncchlbvp.html

head -c 16 /dev/urandom | base64
来源：http://hz.cdnleiting.top/gtcyyznwqa.html

[R70] 时间戳与互转
来源：http://hz.9152youxi.cn/gtbfpjhlhx.html

date +%s;  date -d @1700000000
来源：http://hz.hnxiangtu.top/gtmxraulca.html

[R71] 日期格式化
来源：http://hz.quarkkingdee.top/gtfpigtqmw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shanyushiyangtech.top/gtpwqoklrc.html

[R72] 等待端口就绪
来源：http://hz.birdmap.top/gtargfjxhp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtqwuinvcu.html

[R73] 分割大日志
来源：http://hz.xuanzx.com/gtumqhswhg.html

split -l 1000 big.log part_
来源：http://hz.svipenyu.cn/gtlojmzspg.html

[R74] 批量重命名
来源：http://hz.guannengcc.top/gtlvunotlu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenlongwang.top/gttylggyyu.html

[R75] 导出环境变量
来源：http://hz.birdmap.top/gtpbyxhdem.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xingfuxueyuan.xyz/gtygmrxrcw.html

[R76] 使用临时文件
来源：http://hz.ppjwa.cn/gtctxrfnol.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtvnqeyszq.html

[R77] 读取用户输入
来源：http://hz.sufxvd.cn/gtkpranxhi.html

read -rp "请输入: " ans
来源：http://hz.yvedp.cn/gtzioonvpz.html

[R78] 交互式菜单
来源：http://hz.aizwys.cn/gtjrsvzxrw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.guannengcc.top/gtlyfxjhfz.html

[R79] 解析命令行选项
来源：http://hz.sysykeji.top/gtyhdchqwi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenlongwang.top/gtpgoleknt.html

[R80] 查看脚本执行耗时
来源：http://hz.zycfv.cn/gtmtqwcklu.html

time ./run.sh
来源：http://hz.jinqigufen.top/gtyqjycpye.html

================================================================================
来源：http://hz.zhixingplan.top/gtootxdbak.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gtweclrvya.html

================================================================================
来源：http://hz.hysaishi.cn/gtcfupzogn.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtfqidxcbs.html

#include <stdio.h>
来源：http://hz.gaohongyu789.top/gtzvdhjiln.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jianghu66.top/gtgvvgaohj.html

[S02] C：变量与格式化输出
来源：http://hz.yuxming.cn/gtjbcqivtv.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gtpxkkgigj.html

[S03] C：读入整数
来源：http://hz.wangshuangyany.cn/gtdcfbysmf.html

int x; scanf("%d", &x);
来源：http://hz.yangfankeji.com/gtyggcskfz.html

[S04] C：字符串复制
来源：http://hz.zhijiandao.cn/gtwmrcsemy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guowangkeji.top/gtvyzhfpms.html

[S05] C：字符串长度
来源：http://hz.ydjk.org.cn/gtidpbynui.html

strlen(s)
来源：http://hz.ehwqpu.com/gtnvixxcqh.html

[S06] C：字符串比较
来源：http://hz.ppjwa.cn/gtjqxyrncc.html

strcmp(a, b) == 0
来源：http://hz.yj20258.top/gtpjenysuz.html

[S07] C：数组遍历求和
来源：http://hz.jinqigufen.top/gtmsfnpjid.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gtcehzgikb.html

[S08] C：动态内存分配与释放
来源：http://hz.hnxiangtu.top/gtxelklojy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pycfn.com/gtezrukvih.html

[S09] C：结构体定义与初始化
来源：http://hz.zhongyouzk.top/gttnyxdchu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.birdmap.top/gtfejhzjkb.html

[S10] C：指针与解引用
来源：http://hz.zdqjudy.top/gtaybwlkrk.html

int *p = &a;  *p = 5;
来源：http://hz.hywenlv.cn/gtnnjahgrs.html

[S11] C：逐行读文件
来源：http://hz.feifeiyinyue.top/gtsxslmnor.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xylfe.cn/gtihlndsga.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hfpthk.cn/gtfgeyktqi.html

fclose(f);
来源：http://hz.fengsongda.top/gtdwwefxpa.html

[S12] C：写文件
来源：http://hz.cqqwz.cn/gtoykcxkdj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cucudq.cn/gtgqmsbcii.html

[S13] C：宏定义
来源：http://hz.chenlongwang.top/gteatescbt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinqigufen.top/gtnehkeprj.html

[S14] C：枚举
来源：http://hz.ivvv.top/gthmyjfeew.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tian-w.cn/gtnkbufjbn.html

[S15] C：类型转换
来源：http://hz.gogol.net.cn/gtngmsvnyc.html

(double) a / b
来源：http://hz.jlsjyb.cn/gtqvskznjo.html

[S16] C：位操作置位
来源：http://hz.ydjk.org.cn/gttjhqfbvm.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtcwiopyat.html

[S17] C：安全拼接字符串
来源：http://hz.ppjwa.cn/gtamugykrp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258.top/gtvtcwmumo.html

[S18] C：命令行参数
来源：http://hz.jinghuilouyu.cn/gtvveuprwt.html

int main(int argc, char **argv)
来源：http://hz.yuanzhike.top/gtavwyfjzi.html

[S19] C：快速排序
来源：http://hz.ybcxt.top/gtrynawdfh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.feifeiyinyue.top/gtlxbvebrf.html

[S20] C：二分查找
来源：http://hz.ydjk.org.cn/gtfjxlhrcl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtrpdgnzll.html

[S21] C：字符类别判断
来源：http://hz.jinyuanbaomall.cn/gtdioxxzbk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xinyue.icu/gttnxndvta.html

[S22] C：字符串转数字
来源：http://hz.ydjk.org.cn/gtzcjanfna.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuxming.cn/gtyyymcecs.html

[S23] C：随机数
来源：http://hz.jiagoushi.top/gtieihfuin.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.redwolf501.top/gtmbnhnamv.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangtech.top/gtggdxubvr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxuanxn.top/gttopwfimp.html

[S25] C：内存拷贝
来源：http://hz.tanke756.top/gtuhfzhnyw.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gtwyhfoqrt.html

[S26] C：内存清零
来源：http://hz.jinghuilouyu.cn/gttdrxkgyg.html

memset(a, 0, sizeof a);
来源：http://hz.zhongyouzk.top/gtswprsftg.html

[S27] C：定义常量
来源：http://hz.aibaodan.cn/gtkknqaaac.html

const double PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtrfnjrphd.html

[S28] C：静态变量
来源：http://hz.fengsongda.top/gtyymojoez.html

static int counter = 0;
来源：http://hz.xziqi.cn/gtwmocnznd.html

[S29] C：变参函数
来源：http://hz.dashuyun.cn/gtoooiqrgh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daria6918.cn/gtdobtkjqd.html

[S30] C：头文件保护
来源：http://hz.hywenlv.cn/gtvsscmppy.html

#ifndef X_H
来源：http://hz.jlsjyb.cn/gtziyhhcjx.html

#define X_H
来源：http://hz.smart0.xyz/gtykkwdgpg.html

#endif
来源：http://hz.ehwqpu.com/gtdlopkwum.html

[S31] C++：Hello World
来源：http://hz.smart0.xyz/gtkpnsigoe.html

#include <iostream>
来源：http://hz.yvedp.cn/gttccvtoyd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhengqikj.top/gttregkxxn.html

[S32] C++：字符串
来源：http://hz.yuanzhike.top/gtqnasxfht.html

std::string s = "hi";  s += "!";
来源：http://hz.jiagoushi.top/gtculehzhc.html

[S33] C++：vector 增删
来源：http://hz.zhiwuduotai.top/gtyaeecaxg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sufxvd.cn/gtnqzcaoch.html

[S34] C++：遍历 vector
来源：http://hz.yangfankeji.com/gtubhwyhau.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhengqikj.top/gthulzjsoh.html

[S35] C++：map
来源：http://hz.zhaomingkeji.xyz/gttxlzyrix.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtdoigmlec.html

[S36] C++：unordered_map
来源：http://hz.zhijiandao.cn/gtldzoifmz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtgsapmtzh.html

[S37] C++：set
来源：http://hz.shangyingyoupin.top/gtxwibwznj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.dashuyun.cn/gtjccgszhs.html

[S38] C++：排序
来源：http://hz.316326.xyz/gtxcwrrsuc.html

std::sort(v.begin(), v.end());
来源：http://hz.xziqi.cn/gtuxifuqky.html

[S39] C++：自定义比较器排序
来源：http://hz.vqdsnc.cn/gtguorbtok.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ivvv.top/gtxdvhatxb.html

[S40] C++：查找元素
来源：http://hz.zhoulong.xyz/gthrcekafa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenjidiqi.icu/gtjkxxkpnq.html

[S41] C++：类与构造函数
来源：http://hz.yvedp.cn/gtyzpzyjwg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sweek.top/gtozqjnqfd.html

[S42] C++：继承与虚函数
来源：http://hz.hongshengwenyu.top/gtmfgqoria.html

class B : public Base { public: void f() override {} };
来源：http://hz.gotoacloud.top/gtddcumwxo.html

[S43] C++：智能指针
来源：http://hz.iojbl.cn/gtmtqovjkj.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenzaomai.com/gteietcmri.html

[S44] C++：引用传参
来源：http://hz.zhengqikj.top/gteolhbzjf.html

void inc(int &x) { ++x; }
来源：http://hz.9152youxi.cn/gtwbbmwzei.html

[S45] C++：lambda
来源：http://hz.ywan-chungtsiang.top/gtfkbrggzz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuanzhike.top/gtwvnzluwo.html

[S46] C++：函数模板
来源：http://hz.zhoulong.xyz/gtwfsttkym.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jlsjyb.cn/gtlcjrifqu.html

[S47] C++：结构化绑定遍历
来源：http://hz.hysaishi.cn/gtctufzcxe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgufenzy.top/gtoizqlbrx.html

[S48] C++：逐行读文件
来源：http://hz.ydjk.org.cn/gtcdpnsvci.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hongshengwenyu.top/gtnerfzbre.html

while (std::getline(in, line)) { }
来源：http://hz.ywan-chungtsiang.top/gtmdqtokyd.html

[S49] C++：写文件
来源：http://hz.tian-w.cn/gtxkqhobyd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.iojbl.cn/gtvykehcjs.html

[S50] C++：格式化数字
来源：http://hz.ydjk.org.cn/gtdhpnhurf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtcrinzgvs.html

[S51] C++：显式类型转换
来源：http://hz.jiagoushi.top/gttorixwea.html

static_cast<double>(a) / b
来源：http://hz.aizwys.cn/gtmiskprqj.html

[S52] C++：const 与 noexcept
来源：http://hz.vqdsnc.cn/gtidnjcdvp.html

int size() const noexcept { return n_; }
来源：http://hz.shuidangran.top/gtlkkhpjmy.html

[S53] C++：移动语义
来源：http://hz.tianlin.xyz/gtvpyxlwjq.html

std::vector<int> w = std::move(v);
来源：http://hz.zycfv.cn/gtvsmoavkw.html

[S54] C++：异常处理
来源：http://hz.xylfe.cn/gtdkhnnqpf.html


<!-- 参考信息 -->