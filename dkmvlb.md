代发 wailian999

[Q78] 当前时间
来源：http://hz.shanyushiyangtech.top/gtpyovfrwe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigufen.top/gtgtfrudfg.html

[Q79] 字符串拼接
来源：http://hz.yj20258.top/gtemvxywah.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hfpthk.cn/gtjskbzfyn.html

[Q80] 字符串截取
来源：http://hz.zhijiandao.cn/gtcggelary.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shuidangran.top/gtembvfwre.html

[Q81] 字符串替换
来源：http://hz.chenlongwang.top/gtywwprbvw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dashuyun.cn/gtrypadkvx.html

[Q82] 字符长度与字节长度
来源：http://hz.sysykeji.top/gtpwbojxkd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangdashe.top/gtobfbqofi.html

[Q83] 大小写转换
来源：http://hz.ppjwa.cn/gtkybpkdgw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258.top/gtazgeftik.html

[Q84] 去除首尾空格
来源：http://hz.hysaishi.cn/gtylzvyhpf.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtqojekjpv.html

[Q85] 数值取整
来源：http://hz.hnxiangtu.top/gtylhiovuq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jyoumei.cn/gtlvmndzba.html

[Q86] 读取 JSON 字段
来源：http://hz.andypj.xyz/gtmclozfle.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hfpthk.cn/gtxxycjmry.html

[Q87] JSON 字段做条件
来源：http://hz.tian-w.cn/gtqmpksasl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.snrcjt.cn/gtddvhgksw.html

[Q88] 行转列（条件聚合）
来源：http://hz.fzhhl.top/gtvsusdpfk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.andypj.xyz/gtpzzhtejp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jlsjyb.cn/gtmvhjqoik.html

[Q89] 判断表是否存在
来源：http://hz.aizwys.cn/gtsznehwev.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhoulong.xyz/gtlviaecrc.html

[Q90] 生成序号列
来源：http://hz.ybcxt.top/gtmvlubjcz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yanxiufei.cn/gtlvukapox.html

================================================================================
来源：http://hz.jiagoushi.top/gtavdfmxlu.html

R. Bash 专题
来源：http://hz.ehwqpu.com/gtucwovugo.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtfkdogcom.html

[R01] shebang 与严格模式
来源：http://hz.jqgfzy.top/gtlmzlrhyr.html

#!/usr/bin/env bash
来源：http://hz.zhijiandao.cn/gtpuqpkplt.html

set -euo pipefail
来源：http://hz.chenzaomai.com/gthxmaddij.html

[R02] 变量赋值与使用
来源：http://hz.xziqi.cn/gtkhgnyzpj.html

name="Tom"; echo "$name"
来源：http://hz.zhiwuduotai.top/gthgqawbaa.html

[R03] 只读变量
来源：http://hz.xinyue.icu/gthzajuilx.html

readonly PI=3.14
来源：http://hz.cheryme.top/gttetnyyxa.html

[R04] 位置参数
来源：http://hz.xylfe.cn/gtcxzlreex.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangdashe.top/gtgqegboov.html

[R05] 参数默认值
来源：http://hz.jinyuanbaomall.cn/gtboocxcfo.html

name="${1:-default}"
来源：http://hz.redwolf501.top/gtoyfupdns.html

[R06] 判断命令是否存在
来源：http://hz.yangfankeji.com/gtmrcjflik.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.quarkkingdee.top/gtaftyqvmw.html

[R07] if 判断文件
来源：http://hz.yj202588.top/gthwpunktt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jianghu66.top/gtjxslmzdu.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gteiswcshv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.andypj.xyz/gtjhpcylcv.html

[R09] 字符串比较
来源：http://hz.jqgfzy.top/gtburtabos.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtiqyinswl.html

[R10] 正则匹配
来源：http://hz.svipenyu.cn/gtixgeuhwn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxinkj.top/gtvwbysypa.html

[R11] case 多分支
来源：http://hz.52xcode.cn/gtyogackyr.html

case "$1" in
来源：http://hz.gotoacloud.top/gtjqtepuqq.html

start) echo "启动" ;;
来源：http://hz.cheryme.top/gtfsdqtoir.html

stop)  echo "停止" ;;
来源：http://hz.ehwqpu.com/gtygoveqck.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gtgnypkipp.html

esac
来源：http://hz.nanxuanxn.top/gtsicketqx.html

[R12] for 遍历文件
来源：http://hz.xylfe.cn/gtmwdpxxrj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.iojbl.cn/gtrcgrebtp.html

[R13] for 计数循环
来源：http://hz.hnqzz.top/gtqzbunijf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.haohaochexian.top/gtgokemqfs.html

[R14] C 风格 for
来源：http://hz.hywenlv.cn/gtdyomaklx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtzkjsdaze.html

[R15] while 逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtnvqxzzfa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dashuyun.cn/gtdowgbrcw.html

[R16] until 等待条件
来源：http://hz.birdmap.top/gtlcgwilhd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.snrcjt.cn/gthvmwcimo.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangkeji.top/gtwlbqnmse.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gtvlxazaax.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtgckpbhop.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtbrjdukkq.html

[R19] 数组长度
来源：http://hz.quarkkingdee.top/gtuounepmn.html

echo "${#arr[@]}"
来源：http://hz.0kj1m.cn/gtqeyuizhm.html

[R20] 关联数组（字典）
来源：http://hz.vqdsnc.cn/gtnklxydyt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hfpthk.cn/gtihrwfldq.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtdmolipxv.html

echo "${#s}"
来源：http://hz.zdqjudy.top/gturdbgacq.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gtedcgkepm.html

echo "${s:0:5}"
来源：http://hz.daxiang520.top/gtmvytaesi.html

[R23] 字符串替换
来源：http://hz.yuanzhike.top/gtwbweyjmq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ywan-chungtsiang.top/gtspjbvcig.html

[R24] 大小写转换
来源：http://hz.jinqigufen.top/gtskrpjhpa.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinghuilouyu.cn/gtxrnuzhlh.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinyuanbaomall.cn/gtlzeahyzf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yangfankeji.com/gtatjtvola.html

[R26] 命令替换
来源：http://hz.9152youxi.cn/gtdvsrknau.html

now=$(date +%F); echo "$now"
来源：http://hz.jlsjyb.cn/gtqjzmajzo.html

[R27] 算术展开
来源：http://hz.quarkkingdee.top/gtcdqouypj.html

echo $((1 + 2 * 3))
来源：http://hz.316326.xyz/gtznvuuvwm.html

[R28] 浮点运算
来源：http://hz.316326.xyz/gtttsrcasf.html

echo "scale=2; 10/3" | bc
来源：http://hz.jyoumei.cn/gtbmopfcxt.html

[R29] 定义函数
来源：http://hz.bjfxy.top/gtdpbiyjoz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tian-w.cn/gtampffkjp.html

[R30] 函数返回状态码
来源：http://hz.zhiwuduotai.top/gtvevfmsww.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.snrcjt.cn/gtzegoqazk.html

[R31] 局部变量
来源：http://hz.ywan-chungtsiang.top/gtktfukbnh.html

f() { local x=1; echo "$x"; }
来源：http://hz.gzhubu.top/gtscqhhklg.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtgqtuqktp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shuidangran.top/gtxwvjcoir.html

[R33] 捕获错误并提示行号
来源：http://hz.yangfankeji.com/gtfhyyeknt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sufxvd.cn/gtbhpkgmmy.html

[R34] 退出时清理
来源：http://hz.52xcode.cn/gttpzisopj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtrgbezvpj.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangtech.top/gtokihxczs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pycfn.com/gtkbywldre.html

[R36] 并发执行多个任务
来源：http://hz.jinqigfzy.top/gtespksqxd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.snrcjt.cn/gtdwcmtugr.html

[R37] 把输出赋给变量
来源：http://hz.andypj.xyz/gtcwifcmea.html

files=$(ls -1)
来源：http://hz.hongshengwenyu.top/gtlvpnnjzp.html

[R38] 管道串联
来源：http://hz.cdnleiting.top/gtaunejwis.html

cat a.txt | grep -i error | wc -l
来源：http://hz.havefunace.top/gtllszftdj.html

[R39] 重定向标准输出与错误
来源：http://hz.andypj.xyz/gtzyjblfos.html

cmd > out.log 2>&1
来源：http://hz.c1oappe.top/gtghzkcmbd.html

[R40] 追加写日志
来源：http://hz.gaohongyu789.top/gtpwohnzrd.html

echo "log" >> out.log
来源：http://hz.0kj1m.cn/gtuasoosal.html

[R41] 丢弃输出
来源：http://hz.xuetiantiany.cn/gtrbnwuvoe.html

cmd >/dev/null 2>&1
来源：http://hz.kuanghao11.cn/gtgryzzkgk.html

[R42] 输入重定向
来源：http://hz.shangyingyoupin.top/gtxzrpbbja.html

wc -l < a.txt
来源：http://hz.zdqjudy.top/gtbgbwkhsq.html

[R43] 按名字查找文件
来源：http://hz.aibaodan.cn/gtrxspqvuv.html

find . -name "*.log" -type f
来源：http://hz.zhiwuduotai.top/gthucchiqy.html

[R44] 按修改时间查找
来源：http://hz.yuxming.cn/gtijguixeh.html

find . -mtime -7 -type f
来源：http://hz.ivvv.top/gtftdrxynh.html

[R45] 批量删除
来源：http://hz.cqqwz.cn/gtpwzoejfk.html

find . -name "*.tmp" -delete
来源：http://hz.ywan-chungtsiang.top/gtvnkirtgo.html

[R46] 递归替换文件内容
来源：http://hz.fengsongda.top/gtijqlpuso.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ydjk.org.cn/gtexizhqtn.html

[R47] sed 单行替换
来源：http://hz.shzxlz.cn/gtelbntjyo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.c1oappe.top/gtridfnsnw.html

[R48] awk 取指定列
来源：http://hz.shanyushiyangtech.top/gtlydadwvs.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhiwuduotai.top/gtsmlmzoft.html

[R49] awk 带条件
来源：http://hz.nanxuanxn.top/gtzvdnvovc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhijiandao.cn/gtajlmakvi.html

[R50] awk 求和
来源：http://hz.52xcode.cn/gtxyiqyife.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.haohaochexian.top/gtiymaersx.html

[R51] 排序去重取前几
来源：http://hz.sysykeji.top/gtketajwtq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aizwys.cn/gtqtuculra.html

[R52] 统计行数
来源：http://hz.sxryk.cn/gtgrktplym.html

wc -l a.txt
来源：http://hz.daxiang520.top/gtiujutzfd.html

[R53] 查看文件头与实时尾
来源：http://hz.ywan-chungtsiang.top/gtkvigdqra.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.smart0.xyz/gtldnfrxmv.html

[R54] 比较两个文件
来源：http://hz.xuetiantiany.cn/gtxcvejfsi.html

diff a.txt b.txt
来源：http://hz.aibaodan.cn/gtzlawsxhu.html

[R55] 压缩与解压
来源：http://hz.zhixingplan.top/gtazyzpffq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gaohongyu789.top/gtontgejsg.html

[R56] 远程拷贝
来源：http://hz.cqqwz.cn/gtjoznttpk.html

scp file user@host:/path/
来源：http://hz.gotoacloud.top/gthbpqxbne.html

[R57] 远程执行命令
来源：http://hz.vqdsnc.cn/gtinpxltzk.html

ssh user@host 'uptime'
来源：http://hz.jqgfzy.top/gtysfmunbt.html

[R58] 下载文件
来源：http://hz.zhiwuduotai.top/gtwswmxpwr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shanyushiyangtech.top/gtkdaoukgz.html

[R59] 发 POST JSON
来源：http://hz.jqgfzy.top/gtuwtwpdls.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hammf.cn/gtimmszbjr.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtdhibhxyw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jianghu66.top/gterzgdcjo.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtfbjclfli.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtfnpxlils.html

[R62] 找最占空间的文件
来源：http://hz.zhixingplan.top/gtdxcryqrw.html

du -ah . | sort -rh | head -10
来源：http://hz.yanxiufei.cn/gtlapczcsc.html

[R63] 内存与进程
来源：http://hz.yuxming.cn/gtjaedwcel.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtscawigyq.html

[R64] 结束进程
来源：http://hz.gotoacloud.top/gturueckgf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.aizwys.cn/gtzpmhwubk.html

[R65] 查看端口占用
来源：http://hz.jqgufenzy.top/gttcznyawm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yanxiufei.cn/gthnjwtsji.html

[R66] 定时任务
来源：http://hz.gzhubu.top/gthdevbzrk.html

crontab -e;  crontab -l
来源：http://hz.xuetiantiany.cn/gtgljbhtwg.html

[R67] 生成随机十六进制串
来源：http://hz.guannengcc.top/gtusukrnrr.html

openssl rand -hex 16
来源：http://hz.cashguo.top/gtfcwiltri.html

[R68] 计算文件校验值
来源：http://hz.haohaochexian.top/gtcjeujjft.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hnqzz.top/gtkimygbsl.html

[R69] 生成随机密码
来源：http://hz.yonumen.top/gtboevgvvj.html

head -c 16 /dev/urandom | base64
来源：http://hz.hysaishi.cn/gtfmlrbfrf.html

[R70] 时间戳与互转
来源：http://hz.shuidangran.top/gtaxpltjaa.html

date +%s;  date -d @1700000000
来源：http://hz.haohaochexian.top/gtghnfjbog.html

[R71] 日期格式化
来源：http://hz.zhoulong.xyz/gthpehiupk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxinkj.top/gtnktbhcuc.html

[R72] 等待端口就绪
来源：http://hz.xingfuxueyuan.xyz/gtxxlchimj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zdqjudy.top/gtnvyoxkpe.html

[R73] 分割大日志
来源：http://hz.dianchejie.cn/gtybnlqlxs.html

split -l 1000 big.log part_
来源：http://hz.yonumen.top/gtbnjgnqoe.html

[R74] 批量重命名
来源：http://hz.guannengcc.top/gtnpljkjsc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hammf.cn/gtxrgpsukq.html

[R75] 导出环境变量
来源：http://hz.jlsjyb.cn/gtumosdxjr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhaomingkeji.xyz/gtymywbxyv.html

[R76] 使用临时文件
来源：http://hz.ywan-chungtsiang.top/gtrgzvgddr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtbyyxhspp.html

[R77] 读取用户输入
来源：http://hz.yueranfly.top/gtlihgegbn.html

read -rp "请输入: " ans
来源：http://hz.fzhhl.top/gtqiterjku.html

[R78] 交互式菜单
来源：http://hz.fzhhl.top/gtfuhfzftu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.9152youxi.cn/gtmpqcgsai.html

[R79] 解析命令行选项
来源：http://hz.jiagoushi.top/gtjaozksfk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hywenlv.cn/gtwvbysdop.html

[R80] 查看脚本执行耗时
来源：http://hz.mhx1999.top/gtodmgfuhf.html

time ./run.sh
来源：http://hz.guowangkeji.top/gtepvllasm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtegtymbzj.html

S. C / C++ 专题
来源：http://hz.sxryk.cn/gtcxprguxv.html

================================================================================
来源：http://hz.yangfankeji.com/gtewjqiekt.html

[S01] C：Hello World
来源：http://hz.shanyushiyangkeji.top/gtaxwvsbdr.html

#include <stdio.h>
来源：http://hz.sufxvd.cn/gtkuyhfhte.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shuidangran.top/gtjixfqlcs.html

[S02] C：变量与格式化输出
来源：http://hz.yangfankeji.com/gtameiagod.html

int a = 10; printf("%d\n", a);
来源：http://hz.ybcxt.top/gtdcrgvykp.html

[S03] C：读入整数
来源：http://hz.tian-w.cn/gtypfarzeh.html

int x; scanf("%d", &x);
来源：http://hz.jlsjyb.cn/gtjuysfriy.html

[S04] C：字符串复制
来源：http://hz.hysaishi.cn/gtqrfuajhm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ehwqpu.com/gtrmiqdfmr.html

[S05] C：字符串长度
来源：http://hz.fzhhl.top/gtsjmgkosd.html

strlen(s)
来源：http://hz.gzhubu.top/gtxanwabta.html

[S06] C：字符串比较
来源：http://hz.iojbl.cn/gtonmdlrxi.html

strcmp(a, b) == 0
来源：http://hz.zhoulong.xyz/gttyxdietv.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtpfgvawbs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cqqwz.cn/gtjtalduoq.html

[S08] C：动态内存分配与释放
来源：http://hz.sysykeji.top/gtbwzupqkr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yanxiufei.cn/gtqswqivcx.html

[S09] C：结构体定义与初始化
来源：http://hz.zycfv.cn/gtppbsjjwz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yongpay.top/gtozlqqctk.html

[S10] C：指针与解引用
来源：http://hz.pengpengdd.cyou/gtjlnzxslv.html

int *p = &a;  *p = 5;
来源：http://hz.xylfe.cn/gtisoymivl.html

[S11] C：逐行读文件
来源：http://hz.hammf.cn/gtzabwzoro.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tian-w.cn/gtmwimikjz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.haohaochexian.top/gthycgspzj.html

fclose(f);
来源：http://hz.0kj1m.cn/gtfbkjjbnb.html

[S12] C：写文件
来源：http://hz.0kj1m.cn/gtqlqmgzap.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gzhubu.top/gttzzrocyx.html

[S13] C：宏定义
来源：http://hz.snrcjt.cn/gttkxdwzpt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtwacrxtix.html

[S14] C：枚举
来源：http://hz.yj202588.top/gtgweddcaw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yvedp.cn/gtxddshgie.html

[S15] C：类型转换
来源：http://hz.jianghu66.top/gtpivuxaar.html

(double) a / b
来源：http://hz.jianghu66.top/gtjhdtzmvw.html

[S16] C：位操作置位
来源：http://hz.zhongyouzk.top/gttgmrmxil.html

x |= (1 << 3);
来源：http://hz.nanxinkj.top/gtmnnrbzil.html

[S17] C：安全拼接字符串
来源：http://hz.iojbl.cn/gtgqtcldxc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shangyingyoupin.top/gtjpcqmuwj.html

[S18] C：命令行参数
来源：http://hz.guannengcc.top/gtsoeuzteh.html

int main(int argc, char **argv)
来源：http://hz.jinghuilouyu.cn/gtowcqprml.html

[S19] C：快速排序
来源：http://hz.shuidangran.top/gtivekbyuu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtpaiapdpc.html

[S20] C：二分查找
来源：http://hz.yonumen.top/gtdhobjldb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtpjbbxyyv.html

[S21] C：字符类别判断
来源：http://hz.jlsjyb.cn/gtytxklgdz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aizwys.cn/gtvqrvelrs.html

[S22] C：字符串转数字
来源：http://hz.haohaochexian.top/gtwirtnhoq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hnqzz.top/gtitigjzon.html

[S23] C：随机数
来源：http://hz.yonumen.top/gtccdnhopp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinqigfzy.top/gtvgvhlvza.html

[S24] C：获取本地时间
来源：http://hz.jqgufenzy.top/gtsfezkfck.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cashguo.top/gtwzexxtim.html

[S25] C：内存拷贝
来源：http://hz.tanke756.top/gtczpdcupy.html

memcpy(dst, src, n);
来源：http://hz.xylfe.cn/gtwpnarpdv.html

[S26] C：内存清零
来源：http://hz.gotoacloud.top/gtlmlvnhav.html

memset(a, 0, sizeof a);
来源：http://hz.dashuyun.cn/gtyzplerke.html

[S27] C：定义常量
来源：http://hz.jiagoushi.top/gtkljnnorq.html

const double PI = 3.14159;
来源：http://hz.zycfv.cn/gtzccajscc.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtowwbnspt.html

static int counter = 0;
来源：http://hz.iojbl.cn/gtdnfljcjg.html

[S29] C：变参函数
来源：http://hz.aibaodan.cn/gtlefpkgsp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shuidangran.top/gthiwtlxeg.html

[S30] C：头文件保护
来源：http://hz.wangshuangyany.cn/gtnscmjxme.html

#ifndef X_H
来源：http://hz.gaohongyu789.top/gtsmvejvaz.html

#define X_H
来源：http://hz.zdqjudy.top/gtdnnslxno.html

#endif
来源：http://hz.mhx1999.top/gtnuixewbj.html

[S31] C++：Hello World
来源：http://hz.jinqigufen.top/gtatzyfune.html

#include <iostream>
来源：http://hz.hammf.cn/gttjcazboa.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sufxvd.cn/gtmmmwmoku.html

[S32] C++：字符串
来源：http://hz.jinqigufen.top/gtzopvvxlc.html

std::string s = "hi";  s += "!";
来源：http://hz.cheryme.top/gtwrvfclyg.html

[S33] C++：vector 增删
来源：http://hz.guannengcc.top/gtmtwsagqt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.smart0.xyz/gtyyngnfyh.html

[S34] C++：遍历 vector
来源：http://hz.quarkkingdee.top/gtmsvgetwm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuetiantiany.cn/gttezopngk.html

[S35] C++：map
来源：http://hz.zhoulong.xyz/gtwcxjkoar.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtbhvprbbl.html

[S36] C++：unordered_map
来源：http://hz.zhongyouzk.top/gtwzolwpry.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtzubwbfzs.html

[S37] C++：set
来源：http://hz.kuanghao11.cn/gtxmtimdij.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.0kj1m.cn/gtskulgngw.html

[S38] C++：排序
来源：http://hz.jinghuilouyu.cn/gtosvqagim.html

std::sort(v.begin(), v.end());
来源：http://hz.quarkkingdee.top/gtrderdjgf.html

[S39] C++：自定义比较器排序
来源：http://hz.yuxming.cn/gtyvnjxlwu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daria6918.cn/gttcbsibsw.html

[S40] C++：查找元素
来源：http://hz.haohaochexian.top/gtwsuhhele.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ybcxt.top/gtfgcndgmq.html

[S41] C++：类与构造函数
来源：http://hz.jinghuilouyu.cn/gtomifjhol.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gotoacloud.top/gtzdarvksf.html

[S42] C++：继承与虚函数
来源：http://hz.svipenyu.cn/gtqboyihgq.html

class B : public Base { public: void f() override {} };
来源：http://hz.sysykeji.top/gttailyprg.html

[S43] C++：智能指针
来源：http://hz.ehwqpu.com/gtwthupcgu.html

auto p = std::make_unique<int>(5);
来源：http://hz.smart0.xyz/gtufeqjdjp.html

[S44] C++：引用传参
来源：http://hz.ydzc1.top/gtcgmsgoba.html

void inc(int &x) { ++x; }
来源：http://hz.fzhhl.top/gtdqpsckqp.html

[S45] C++：lambda
来源：http://hz.smart0.xyz/gtilwybttv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gtuolueefn.html

[S46] C++：函数模板
来源：http://hz.jinyuanbaomall.cn/gtbrmriath.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinqigufen.top/gtjkusnlmy.html

[S47] C++：结构化绑定遍历
来源：http://hz.yueranfly.top/gtwdvltnsd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.iojbl.cn/gtfstbwamo.html

[S48] C++：逐行读文件
来源：http://hz.snrcjt.cn/gtrgwtsxvy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtqsevvubx.html


<!-- 参考信息 -->