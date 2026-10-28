代发 wailian999

[Q78] 当前时间
来源：http://hz.zhoulong.xyz/gtvbkujlxf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cqqwz.cn/gtvzxgrrzh.html

[Q79] 字符串拼接
来源：http://hz.zdqjudy.top/gtmylxqdby.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigufen.top/gtqvwbopvp.html

[Q80] 字符串截取
来源：http://hz.yj20258888.top/gtueaxcrks.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dashuyun.cn/gtrxidmgrc.html

[Q81] 字符串替换
来源：http://hz.cheryme.top/gtiwqydait.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydzc1.top/gtijtwiezv.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigfzy.top/gtjrikhhwc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gtgpqwmves.html

[Q83] 大小写转换
来源：http://hz.cucudq.cn/gthpudclrw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aizwys.cn/gtqnujhmwy.html

[Q84] 去除首尾空格
来源：http://hz.zhiwuduotai.top/gtirtlkwmm.html

SELECT TRIM(name) FROM users;
来源：http://hz.daria6918.cn/gtwklawuxm.html

[Q85] 数值取整
来源：http://hz.hywenlv.cn/gtwozzqyjo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pycfn.com/gtdzggtueg.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtnlkrxyrz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.smart0.xyz/gtpwzktgbk.html

[Q87] JSON 字段做条件
来源：http://hz.chenzaomai.com/gtgketxqbh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gaohongyu789.top/gtbjjrerdv.html

[Q88] 行转列（条件聚合）
来源：http://hz.pengpengdd.cyou/gtofqfjjoy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gtqcgjzose.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jlsjyb.cn/gturfrprvf.html

[Q89] 判断表是否存在
来源：http://hz.ppjwa.cn/gttshqoavm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgufenzy.top/gtdhoabaqm.html

[Q90] 生成序号列
来源：http://hz.shuidangran.top/gtqtrlpnvz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenlongwang.top/gtwbajiovp.html

================================================================================
来源：http://hz.ehwqpu.com/gtovfdyvjj.html

R. Bash 专题
来源：http://hz.jiagoushi.top/gtublswqcs.html

================================================================================
来源：http://hz.316326.xyz/gtgxdszubo.html

[R01] shebang 与严格模式
来源：http://hz.hysaishi.cn/gtcjrtahdy.html

#!/usr/bin/env bash
来源：http://hz.smart0.xyz/gtdleycbmv.html

set -euo pipefail
来源：http://hz.ybcxt.top/gtzsmgwpwm.html

[R02] 变量赋值与使用
来源：http://hz.yongpay.top/gtiwhptcds.html

name="Tom"; echo "$name"
来源：http://hz.xuanzx.com/gtastuyfex.html

[R03] 只读变量
来源：http://hz.hywenlv.cn/gtplsyxsde.html

readonly PI=3.14
来源：http://hz.shanyushiyangkeji.top/gthnardlyg.html

[R04] 位置参数
来源：http://hz.wangdashe.top/gtolanepde.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ppjwa.cn/gtzsgzsucq.html

[R05] 参数默认值
来源：http://hz.52xcode.cn/gtsrkvjzru.html

name="${1:-default}"
来源：http://hz.haohaochexian.top/gtvfvffjoy.html

[R06] 判断命令是否存在
来源：http://hz.ppjwa.cn/gtjvipcnig.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.birdmap.top/gtmyjynkzr.html

[R07] if 判断文件
来源：http://hz.yj202588.top/gtbehdvdiu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ydzc1.top/gtcjmeyfff.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtploatdra.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yonumen.top/gtkaazmbgt.html

[R09] 字符串比较
来源：http://hz.jinghuilouyu.cn/gtgadmtppe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj202588.top/gtctongvyb.html

[R10] 正则匹配
来源：http://hz.tanke756.top/gtxokqjhdt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gaohongyu789.top/gtyhntzrbo.html

[R11] case 多分支
来源：http://hz.fengsongda.top/gtqzosszoz.html

case "$1" in
来源：http://hz.c1oappe.top/gtlxugcron.html

start) echo "启动" ;;
来源：http://hz.wangdashe.top/gtuxzxfasf.html

stop)  echo "停止" ;;
来源：http://hz.mhx1999.top/gtosrsxsja.html

*)     echo "未知命令" ;;
来源：http://hz.yueranfly.top/gtkkygdqtb.html

esac
来源：http://hz.jiagoushi.top/gtdhtlsljy.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangtech.top/gtzeyjryqf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gtxgfoqpjw.html

[R13] for 计数循环
来源：http://hz.ydjk.org.cn/gtuqkoceqh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sufxvd.cn/gtljushvsh.html

[R14] C 风格 for
来源：http://hz.yanxiufei.cn/gtautexcil.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tanke756.top/gthhkparij.html

[R15] while 逐行读文件
来源：http://hz.gzhubu.top/gtlcxvrgru.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fzhhl.top/gtktdcfioo.html

[R16] until 等待条件
来源：http://hz.kuanghao11.cn/gtzpjsyxob.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxuanxn.top/gthowdrndg.html

[R17] 数组定义与取值
来源：http://hz.zdqjudy.top/gtetxeyamh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhongyouzk.top/gthlgppjix.html

[R18] 遍历数组
来源：http://hz.pengpengdd.cyou/gtscujezfx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sxryk.cn/gtprqykurx.html

[R19] 数组长度
来源：http://hz.cucudq.cn/gtpcyhiesl.html

echo "${#arr[@]}"
来源：http://hz.xinyue.icu/gtprexvocw.html

[R20] 关联数组（字典）
来源：http://hz.zycfv.cn/gtpybvenpm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258.top/gtfmydgbjk.html

[R21] 字符串长度
来源：http://hz.9152youxi.cn/gtjosgqlyr.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtbvgffaeq.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtadrpjkhe.html

echo "${s:0:5}"
来源：http://hz.hysaishi.cn/gtrciytaug.html

[R23] 字符串替换
来源：http://hz.gzhubu.top/gtajydsfzg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.vqdsnc.cn/gtgmvahndq.html

[R24] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtgxdgogys.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yanxiufei.cn/gtpiwdmdda.html

[R25] 去后缀 / 去前缀
来源：http://hz.yonumen.top/gttalxcvli.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ywan-chungtsiang.top/gtcdwwzfeo.html

[R26] 命令替换
来源：http://hz.shanyushiyangtech.top/gtlgxezycw.html

now=$(date +%F); echo "$now"
来源：http://hz.jiagoushi.top/gtazdhwddf.html

[R27] 算术展开
来源：http://hz.yangfankeji.com/gtlfztusyu.html

echo $((1 + 2 * 3))
来源：http://hz.tianlin.xyz/gttrbwrrbk.html

[R28] 浮点运算
来源：http://hz.kuanghao11.cn/gttkcxucvg.html

echo "scale=2; 10/3" | bc
来源：http://hz.guannengcc.top/gtuidkycgz.html

[R29] 定义函数
来源：http://hz.ywan-chungtsiang.top/gtntmyswot.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtiiibbcza.html

[R30] 函数返回状态码
来源：http://hz.xylfe.cn/gttgljkxch.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenjidiqi.icu/gtfnbxcfgw.html

[R31] 局部变量
来源：http://hz.xuetiantiany.cn/gtmkywmbsf.html

f() { local x=1; echo "$x"; }
来源：http://hz.smart0.xyz/gthglaobhv.html

[R32] 参数个数校验
来源：http://hz.zhijiandao.cn/gtxsbksvcl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtgrnbhndi.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gthftyjuxp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtfshgkhdj.html

[R34] 退出时清理
来源：http://hz.yj20258888.top/gtjobixmif.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtrrwloyao.html

[R35] 后台执行并等待
来源：http://hz.fengsongda.top/gtixlqmuoe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sweek.top/gtcdbgbbol.html

[R36] 并发执行多个任务
来源：http://hz.316326.xyz/gtvvodmzfv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cdnleiting.top/gtiwskmswe.html

[R37] 把输出赋给变量
来源：http://hz.hfpthk.cn/gttsuoocjg.html

files=$(ls -1)
来源：http://hz.dianchejie.cn/gtpveqbqdi.html

[R38] 管道串联
来源：http://hz.haohaochexian.top/gtpxvhcjvt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tianlin.xyz/gtijhldaml.html

[R39] 重定向标准输出与错误
来源：http://hz.zhijiandao.cn/gtjlrxdjyl.html

cmd > out.log 2>&1
来源：http://hz.wangdashe.top/gtscjpzycs.html

[R40] 追加写日志
来源：http://hz.feifeiyinyue.top/gttbeodlla.html

echo "log" >> out.log
来源：http://hz.daria6918.cn/gtpaayffbw.html

[R41] 丢弃输出
来源：http://hz.ydzc1.top/gtccofulsh.html

cmd >/dev/null 2>&1
来源：http://hz.snrcjt.cn/gtbqmvnkja.html

[R42] 输入重定向
来源：http://hz.yj202588.top/gtuocvzkpm.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gtbipjdcij.html

[R43] 按名字查找文件
来源：http://hz.quarkkingdee.top/gtlshigqyl.html

find . -name "*.log" -type f
来源：http://hz.jlsjyb.cn/gteprninfx.html

[R44] 按修改时间查找
来源：http://hz.tanke756.top/gtimawfvcf.html

find . -mtime -7 -type f
来源：http://hz.havefunace.top/gtwuvfzwal.html

[R45] 批量删除
来源：http://hz.zdqjudy.top/gtelzzlhlr.html

find . -name "*.tmp" -delete
来源：http://hz.yj202588.top/gtjnwxnbpc.html

[R46] 递归替换文件内容
来源：http://hz.vqdsnc.cn/gtorrlhysc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxinkj.top/gtipvhszhr.html

[R47] sed 单行替换
来源：http://hz.bjfxy.top/gtlxwgnxut.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.svipenyu.cn/gtjstojycn.html

[R48] awk 取指定列
来源：http://hz.mhx1999.top/gtlwixktwe.html

awk '{print $1, $3}' a.txt
来源：http://hz.tanke756.top/gtsfndmpoj.html

[R49] awk 带条件
来源：http://hz.jqgfzy.top/gtutfvpuid.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangdashe.top/gtqwdnpagn.html

[R50] awk 求和
来源：http://hz.pycfn.com/gtxithqyet.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtiigiquve.html

[R51] 排序去重取前几
来源：http://hz.yuxming.cn/gtfdfgfpfp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.andypj.xyz/gtbwywptyd.html

[R52] 统计行数
来源：http://hz.zhiwuduotai.top/gtyyxfkfjx.html

wc -l a.txt
来源：http://hz.jinyuanbaomall.cn/gtqhfkjhsn.html

[R53] 查看文件头与实时尾
来源：http://hz.bjfxy.top/gtczktpyev.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sufxvd.cn/gtvosoqebi.html

[R54] 比较两个文件
来源：http://hz.jlsjyb.cn/gtsvawtqph.html

diff a.txt b.txt
来源：http://hz.nanxinkj.top/gtkjyrowev.html

[R55] 压缩与解压
来源：http://hz.ehwqpu.com/gtxwzptgdl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sxryk.cn/gtebtpcnnb.html

[R56] 远程拷贝
来源：http://hz.xinyue.icu/gtltlzorgc.html

scp file user@host:/path/
来源：http://hz.fzhhl.top/gtsmgiakvl.html

[R57] 远程执行命令
来源：http://hz.fzhhl.top/gtvzcbkraa.html

ssh user@host 'uptime'
来源：http://hz.iojbl.cn/gtykimaspx.html

[R58] 下载文件
来源：http://hz.snrcjt.cn/gtfxzlirrv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sxryk.cn/gtyeofkqnv.html

[R59] 发 POST JSON
来源：http://hz.zdqjudy.top/gtpqqzhhgj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydjk.org.cn/gtnbxpumgx.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtsadkgzwt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.aizwys.cn/gtjsmrhvob.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtkapwtxgu.html

df -h;  du -sh *
来源：http://hz.birdmap.top/gtcuylqskq.html

[R62] 找最占空间的文件
来源：http://hz.jlsjyb.cn/gtdbqzcaky.html

du -ah . | sort -rh | head -10
来源：http://hz.yanxiufei.cn/gtuwojpcmc.html

[R63] 内存与进程
来源：http://hz.ehwqpu.com/gtwuyfpvkd.html

free -h;  ps aux | grep nginx
来源：http://hz.shzxlz.cn/gtufcjtniq.html

[R64] 结束进程
来源：http://hz.wangshuangyany.cn/gtywovfhny.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ppjwa.cn/gtebrkmdvq.html

[R65] 查看端口占用
来源：http://hz.ybcxt.top/gtvvqqmpnl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aibaodan.cn/gtbctpjzon.html

[R66] 定时任务
来源：http://hz.redwolf501.top/gtpgujemtp.html

crontab -e;  crontab -l
来源：http://hz.yvedp.cn/gteupbrkum.html

[R67] 生成随机十六进制串
来源：http://hz.guowangkeji.top/gtdmhchrep.html

openssl rand -hex 16
来源：http://hz.yanxiufei.cn/gtsppxpagm.html

[R68] 计算文件校验值
来源：http://hz.gotoacloud.top/gtcvcxxaht.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenzaomai.com/gthnrqtnea.html

[R69] 生成随机密码
来源：http://hz.hfpthk.cn/gtofvzgiji.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhixingplan.top/gtiykyavas.html

[R70] 时间戳与互转
来源：http://hz.guannengcc.top/gthbtqjsti.html

date +%s;  date -d @1700000000
来源：http://hz.cqqwz.cn/gtngmipcmq.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gttvdrbxba.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhongyouzk.top/gtncxiwwhp.html

[R72] 等待端口就绪
来源：http://hz.kuanghao11.cn/gtgseevpau.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xinyue.icu/gtgdsfyqfl.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gtfevjrqzt.html

split -l 1000 big.log part_
来源：http://hz.hywenlv.cn/gtjbozwiga.html

[R74] 批量重命名
来源：http://hz.yongpay.top/gtxhuscrtw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guannengcc.top/gtvdfgzpmk.html

[R75] 导出环境变量
来源：http://hz.zhoulong.xyz/gtlryseeup.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.smart0.xyz/gtzewpmycf.html

[R76] 使用临时文件
来源：http://hz.sxryk.cn/gtpqxclnbe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhongyouzk.top/gtxmnzbmiv.html

[R77] 读取用户输入
来源：http://hz.yangfankeji.com/gtxnlvnhph.html

read -rp "请输入: " ans
来源：http://hz.zdqjudy.top/gtvkpivjil.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtertkzgmv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.0kj1m.cn/gtgkusjyzi.html

[R79] 解析命令行选项
来源：http://hz.haohaochexian.top/gtyujjtrjm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.bjfxy.top/gtxjxiruzu.html

[R80] 查看脚本执行耗时
来源：http://hz.hywenlv.cn/gtfvzhyjpq.html

time ./run.sh
来源：http://hz.snrcjt.cn/gtikvvsida.html

================================================================================
来源：http://hz.gaohongyu789.top/gtepnavarq.html

S. C / C++ 专题
来源：http://hz.tian-w.cn/gtnxfavpwo.html

================================================================================
来源：http://hz.zhixingplan.top/gtgakfmoyw.html

[S01] C：Hello World
来源：http://hz.xinyue.icu/gtdmybzyww.html

#include <stdio.h>
来源：http://hz.ydzc1.top/gtafwdqlzh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.birdmap.top/gtpgpnlmed.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangkeji.top/gtblpslsum.html

int a = 10; printf("%d\n", a);
来源：http://hz.gotoacloud.top/gtedwjczkb.html

[S03] C：读入整数
来源：http://hz.yuanzhike.top/gttjuxrnws.html

int x; scanf("%d", &x);
来源：http://hz.xuanzx.com/gtghivdowo.html

[S04] C：字符串复制
来源：http://hz.nanxuanxn.top/gtrryslcqk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.vqdsnc.cn/gtbnskyqpk.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtffzokcjo.html

strlen(s)
来源：http://hz.pycfn.com/gthigjntyo.html

[S06] C：字符串比较
来源：http://hz.jlsjyb.cn/gtxhangdts.html

strcmp(a, b) == 0
来源：http://hz.cheryme.top/gteacrvocg.html

[S07] C：数组遍历求和
来源：http://hz.meibo888.top/gthgyadxsc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yuxming.cn/gtqsjexouf.html

[S08] C：动态内存分配与释放
来源：http://hz.hammf.cn/gtoyufpqye.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yvedp.cn/gthhvzpzxw.html

[S09] C：结构体定义与初始化
来源：http://hz.yangfankeji.com/gtwvxwuhoa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.birdmap.top/gtszawteaw.html

[S10] C：指针与解引用
来源：http://hz.guannengcc.top/gtqwhmawot.html

int *p = &a;  *p = 5;
来源：http://hz.yongpay.top/gtzlmssnxo.html

[S11] C：逐行读文件
来源：http://hz.aizwys.cn/gttjqerwwi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtglwfpxbz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.haohaochexian.top/gtmonfcfty.html

fclose(f);
来源：http://hz.hywenlv.cn/gtclmhsqxq.html

[S12] C：写文件
来源：http://hz.aibaodan.cn/gtwmlrvmwf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cheryme.top/gtiivssnsr.html

[S13] C：宏定义
来源：http://hz.pengpengdd.cyou/gtwrmbrnib.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.svipenyu.cn/gtjclnqckw.html

[S14] C：枚举
来源：http://hz.hfpthk.cn/gtruxrguwy.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gttohnpxok.html

[S15] C：类型转换
来源：http://hz.ehwqpu.com/gtssjwirot.html

(double) a / b
来源：http://hz.yonumen.top/gtknaegohd.html

[S16] C：位操作置位
来源：http://hz.ywan-chungtsiang.top/gtddacfkha.html

x |= (1 << 3);
来源：http://hz.yvedp.cn/gtqzhqmnmn.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtxvcjptqa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hysaishi.cn/gtfmqfcnjo.html

[S18] C：命令行参数
来源：http://hz.zhixingplan.top/gtmelsuyxx.html

int main(int argc, char **argv)
来源：http://hz.wangshuangyany.cn/gtrosedziz.html

[S19] C：快速排序
来源：http://hz.jyoumei.cn/gtdczjrzlj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gtotwsavsq.html

[S20] C：二分查找
来源：http://hz.wangdashe.top/gtnmoejthp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhixingplan.top/gtltavjffx.html

[S21] C：字符类别判断
来源：http://hz.yvedp.cn/gtategwshf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daxiang520.top/gtyqirbqoi.html

[S22] C：字符串转数字
来源：http://hz.xylfe.cn/gtdexwzjwf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ywan-chungtsiang.top/gtcanpykau.html

[S23] C：随机数
来源：http://hz.ppjwa.cn/gtciwhrmwf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cdnleiting.top/gtnrsfktur.html

[S24] C：获取本地时间
来源：http://hz.snrcjt.cn/gtazvyfuuf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.316326.xyz/gtyokealzf.html

[S25] C：内存拷贝
来源：http://hz.havefunace.top/gtamkxtfgr.html

memcpy(dst, src, n);
来源：http://hz.feifeiyinyue.top/gtzqetwiib.html

[S26] C：内存清零
来源：http://hz.gaohongyu789.top/gtlnryfisf.html

memset(a, 0, sizeof a);
来源：http://hz.ivvv.top/gtndfaugjx.html

[S27] C：定义常量
来源：http://hz.chenlongwang.top/gtrnfivlay.html

const double PI = 3.14159;
来源：http://hz.ybcxt.top/gtoovgysjp.html

[S28] C：静态变量
来源：http://hz.ybcxt.top/gtqtxvxruk.html

static int counter = 0;
来源：http://hz.pycfn.com/gtwqutxnxs.html

[S29] C：变参函数
来源：http://hz.jyoumei.cn/gtomofwvhj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xziqi.cn/gtfjymwcwy.html

[S30] C：头文件保护
来源：http://hz.smart0.xyz/gtvyifuugm.html

#ifndef X_H
来源：http://hz.tian-w.cn/gtsnpzlqfz.html

#define X_H
来源：http://hz.daxiang520.top/gtfrxnbwtb.html

#endif
来源：http://hz.andypj.xyz/gtlntapvlr.html

[S31] C++：Hello World
来源：http://hz.yueranfly.top/gtbsennluo.html

#include <iostream>
来源：http://hz.nanxinkj.top/gtujkffxzz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuetiantiany.cn/gtkcqyzjpn.html

[S32] C++：字符串
来源：http://hz.yuxming.cn/gtxntiwitk.html

std::string s = "hi";  s += "!";
来源：http://hz.shangyingyoupin.top/gteumdmwld.html

[S33] C++：vector 增删
来源：http://hz.meibo888.top/gtdqsvefpd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.daxiang520.top/gtsuasrxnx.html

[S34] C++：遍历 vector
来源：http://hz.aizwys.cn/gtdbbnoowq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydjk.org.cn/gtxpvvhxts.html

[S35] C++：map
来源：http://hz.jiagoushi.top/gtaszayhvg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhengqikj.top/gtoehvaznm.html

[S36] C++：unordered_map
来源：http://hz.zhengqikj.top/gtlvnkbbgs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gtvvuskvcl.html

[S37] C++：set
来源：http://hz.52xcode.cn/gtkurrjotz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xylfe.cn/gtjefjkcin.html

[S38] C++：排序
来源：http://hz.wangdashe.top/gtwpczlwmg.html

std::sort(v.begin(), v.end());
来源：http://hz.shzxlz.cn/gtchesljkj.html

[S39] C++：自定义比较器排序
来源：http://hz.tanke756.top/gtcjtrynyc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangdashe.top/gtctikpbza.html

[S40] C++：查找元素
来源：http://hz.svipenyu.cn/gtszvdkcni.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ivvv.top/gtgrxwgmpt.html

[S41] C++：类与构造函数
来源：http://hz.snrcjt.cn/gtxbvjatdn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tian-w.cn/gtnqzgkawm.html

[S42] C++：继承与虚函数
来源：http://hz.hfpthk.cn/gtywdigoco.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangtech.top/gtoxbzaxag.html

[S43] C++：智能指针
来源：http://hz.xuanzx.com/gtlaearkhg.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtlysdcmrn.html

[S44] C++：引用传参
来源：http://hz.xylfe.cn/gtdnmbkkvh.html

void inc(int &x) { ++x; }
来源：http://hz.sxryk.cn/gtlputkifd.html

[S45] C++：lambda
来源：http://hz.daxiang520.top/gthykdvgda.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.feifeiyinyue.top/gttvsccugb.html

[S46] C++：函数模板
来源：http://hz.jqgufenzy.top/gtabbvfurq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.bjfxy.top/gttwioqaql.html

[S47] C++：结构化绑定遍历
来源：http://hz.jyoumei.cn/gtuvzpdfti.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.snrcjt.cn/gtnpotczhz.html

[S48] C++：逐行读文件
来源：http://hz.yueranfly.top/gtjikybnlp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.0kj1m.cn/gtyqopjaih.html


<!-- 参考信息 -->