代发 wailian999

SHOW INDEX FROM users;
来源：http://hz.sufxvd.cn/gtdowioxju.html

[Q73] 查看表状态
来源：http://hz.cucudq.cn/gtlvfdagcq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangtech.top/gtnhulxtdz.html

[Q74] 强制使用索引
来源：http://hz.fzhhl.top/gtybnoxvzd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dashuyun.cn/gtujuzwpfc.html

[Q75] 日期格式化
来源：http://hz.yuanzhike.top/gtnnlbtmgs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gzhubu.top/gtidbqzgdk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xziqi.cn/gtlqvfrgmm.html

[Q76] 按天统计
来源：http://hz.yuanzhike.top/gtstazbxme.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gogol.net.cn/gtssqfcnir.html

[Q77] 时间加减
来源：http://hz.hywenlv.cn/gtfiflmhyi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.meibo888.top/gtciktwrhi.html

[Q78] 当前时间
来源：http://hz.zycfv.cn/gtrzskrxbb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gogol.net.cn/gtzexzgxjd.html

[Q79] 字符串拼接
来源：http://hz.zhijiandao.cn/gtrzvnlwmx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sysykeji.top/gtfirojdok.html

[Q80] 字符串截取
来源：http://hz.ydjk.org.cn/gtdmhhyfcc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.birdmap.top/gtkkoyvwfk.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gttlsdntan.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.snrcjt.cn/gtkofyfdly.html

[Q82] 字符长度与字节长度
来源：http://hz.smart0.xyz/gtbuavuyne.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jyoumei.cn/gtuvglxvlt.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtplxgakmq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtcffwetcu.html

[Q84] 去除首尾空格
来源：http://hz.dianchejie.cn/gtuwaohpvx.html

SELECT TRIM(name) FROM users;
来源：http://hz.hfpthk.cn/gtppyjffwc.html

[Q85] 数值取整
来源：http://hz.shanyushiyangtech.top/gthsevupzi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dianchejie.cn/gtyrwdgfin.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxuanxn.top/gtmucacdya.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yuxming.cn/gtvplgzvfn.html

[Q87] JSON 字段做条件
来源：http://hz.guannengcc.top/gtemvlfnkd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.kuanghao11.cn/gtfaqsrcmg.html

[Q88] 行转列（条件聚合）
来源：http://hz.jqgufenzy.top/gtkwcoivug.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ehwqpu.com/gtrrofytvw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenlongwang.top/gthybwoyoi.html

[Q89] 判断表是否存在
来源：http://hz.zdqjudy.top/gtpbnqlvjl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj202588.top/gtxipbplvm.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtqnxrqcwa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yangfankeji.com/gtygdoqgzr.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmveimvpi.html

R. Bash 专题
来源：http://hz.feifeiyinyue.top/gtyfzjxxit.html

================================================================================
来源：http://hz.fzhhl.top/gtpohthjqw.html

[R01] shebang 与严格模式
来源：http://hz.yj202588.top/gtdujrptnf.html

#!/usr/bin/env bash
来源：http://hz.gotoacloud.top/gtqgmstqqg.html

set -euo pipefail
来源：http://hz.yongpay.top/gtuseavvmx.html

[R02] 变量赋值与使用
来源：http://hz.xuanzx.com/gtlnovqxur.html

name="Tom"; echo "$name"
来源：http://hz.hongshengwenyu.top/gtzvsiwqay.html

[R03] 只读变量
来源：http://hz.hnxiangtu.top/gtscrysqcd.html

readonly PI=3.14
来源：http://hz.sweek.top/gtzbebopcy.html

[R04] 位置参数
来源：http://hz.gzhubu.top/gtglwxadus.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gogol.net.cn/gtuzjibvrl.html

[R05] 参数默认值
来源：http://hz.jinghuilouyu.cn/gtyxrkanke.html

name="${1:-default}"
来源：http://hz.9152youxi.cn/gteyujevaa.html

[R06] 判断命令是否存在
来源：http://hz.52xcode.cn/gtvadbonxm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tanke756.top/gtdytqdywh.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtbkoeewoh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.mhx1999.top/gtocshyelt.html

[R08] 数值比较
来源：http://hz.guannengcc.top/gtvryohfhd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daxiang520.top/gtxpunhuja.html

[R09] 字符串比较
来源：http://hz.daxiang520.top/gtzspzuigm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.9152youxi.cn/gtbhhrxtwd.html

[R10] 正则匹配
来源：http://hz.chenjidiqi.icu/gtjvomxgjf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.smart0.xyz/gtlwxnlktz.html

[R11] case 多分支
来源：http://hz.hongshengwenyu.top/gtdhxczoct.html

case "$1" in
来源：http://hz.sysykeji.top/gtohburbso.html

start) echo "启动" ;;
来源：http://hz.jinghuilouyu.cn/gthnmymsfx.html

stop)  echo "停止" ;;
来源：http://hz.hnqzz.top/gtapxuykgo.html

*)     echo "未知命令" ;;
来源：http://hz.ywan-chungtsiang.top/gtpzsremui.html

esac
来源：http://hz.jyoumei.cn/gtiemblbel.html

[R12] for 遍历文件
来源：http://hz.c1oappe.top/gtsvzyadcq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgufenzy.top/gtgqemkfwf.html

[R13] for 计数循环
来源：http://hz.quarkkingdee.top/gtgvydqrlb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yueranfly.top/gtxlbwpefx.html

[R14] C 风格 for
来源：http://hz.xinyue.icu/gtjsoujist.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sysykeji.top/gtlywwsbwz.html

[R15] while 逐行读文件
来源：http://hz.gogol.net.cn/gtfemiliig.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yueranfly.top/gtooiewuul.html

[R16] until 等待条件
来源：http://hz.yanxiufei.cn/gtqgofpdhr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sweek.top/gtfifxebsy.html

[R17] 数组定义与取值
来源：http://hz.bjfxy.top/gtqjksvzbc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cucudq.cn/gtpvqujopp.html

[R18] 遍历数组
来源：http://hz.xingfuxueyuan.xyz/gtqqzdznhl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuanzhike.top/gtyflhhzsj.html

[R19] 数组长度
来源：http://hz.jinyuanbaomall.cn/gtmeqkidli.html

echo "${#arr[@]}"
来源：http://hz.cucudq.cn/gtwrrbvgee.html

[R20] 关联数组（字典）
来源：http://hz.fengsongda.top/gtztblmfmh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hfpthk.cn/gtxgwgfqah.html

[R21] 字符串长度
来源：http://hz.redwolf501.top/gthmjtsada.html

echo "${#s}"
来源：http://hz.svipenyu.cn/gtpoeveymx.html

[R22] 截取子串
来源：http://hz.zhijiandao.cn/gticwgfugl.html

echo "${s:0:5}"
来源：http://hz.yj20258.top/gtdcpaxzcf.html

[R23] 字符串替换
来源：http://hz.iojbl.cn/gtwniurond.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jiagoushi.top/gtvtucgwrp.html

[R24] 大小写转换
来源：http://hz.guowangkeji.top/gteavfcdqb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258.top/gtrqgobmdk.html

[R25] 去后缀 / 去前缀
来源：http://hz.pengpengdd.cyou/gtupihfmgy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.mhx1999.top/gtzoptkxke.html

[R26] 命令替换
来源：http://hz.smart0.xyz/gtceaiadoo.html

now=$(date +%F); echo "$now"
来源：http://hz.zycfv.cn/gtilntsdjc.html

[R27] 算术展开
来源：http://hz.hfpthk.cn/gtrcnnqxov.html

echo $((1 + 2 * 3))
来源：http://hz.gotoacloud.top/gtnthlvctg.html

[R28] 浮点运算
来源：http://hz.xingfuxueyuan.xyz/gtreklpnmt.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtzengmase.html

[R29] 定义函数
来源：http://hz.chenjidiqi.icu/gtkbdxohac.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhoulong.xyz/gtsvtpdfyw.html

[R30] 函数返回状态码
来源：http://hz.daxiang520.top/gtjfmdmaxa.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gtnorodoxu.html

[R31] 局部变量
来源：http://hz.jinqigufen.top/gtkpxbnrsg.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenlongwang.top/gtqysjazfp.html

[R32] 参数个数校验
来源：http://hz.zhengqikj.top/gtkovmqkne.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.bjfxy.top/gtspfhmxow.html

[R33] 捕获错误并提示行号
来源：http://hz.cdnleiting.top/gtpaazrgah.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigfzy.top/gtesznqoho.html

[R34] 退出时清理
来源：http://hz.sxryk.cn/gtjkaulxhr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtmtkhkjcy.html

[R35] 后台执行并等待
来源：http://hz.chenlongwang.top/gtzoglmnnv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xingfuxueyuan.xyz/gtuaxopljs.html

[R36] 并发执行多个任务
来源：http://hz.yuanzhike.top/gtfpdsevra.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenjidiqi.icu/gtaszboeuz.html

[R37] 把输出赋给变量
来源：http://hz.jqgufenzy.top/gtuwewwrhp.html

files=$(ls -1)
来源：http://hz.cashguo.top/gtyzkpcyse.html

[R38] 管道串联
来源：http://hz.haohaochexian.top/gtlcxcxvpj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cashguo.top/gtvvntvkqg.html

[R39] 重定向标准输出与错误
来源：http://hz.316326.xyz/gtmhxrunvc.html

cmd > out.log 2>&1
来源：http://hz.zhoulong.xyz/gtnyakknsn.html

[R40] 追加写日志
来源：http://hz.tianlin.xyz/gtqlzglsgt.html

echo "log" >> out.log
来源：http://hz.andypj.xyz/gtlnkylaeu.html

[R41] 丢弃输出
来源：http://hz.jqgufenzy.top/gtmckkwcjs.html

cmd >/dev/null 2>&1
来源：http://hz.yongpay.top/gtnnodyjtr.html

[R42] 输入重定向
来源：http://hz.316326.xyz/gtjgurvcha.html

wc -l < a.txt
来源：http://hz.daria6918.cn/gtmkaexptz.html

[R43] 按名字查找文件
来源：http://hz.iojbl.cn/gtcugqkhit.html

find . -name "*.log" -type f
来源：http://hz.yj20258.top/gtcvprymvo.html

[R44] 按修改时间查找
来源：http://hz.havefunace.top/gtwluclxot.html

find . -mtime -7 -type f
来源：http://hz.jinyuanbaomall.cn/gtgtcpdgfe.html

[R45] 批量删除
来源：http://hz.zycfv.cn/gtnxxraoci.html

find . -name "*.tmp" -delete
来源：http://hz.shangyingyoupin.top/gtbrbjsoxp.html

[R46] 递归替换文件内容
来源：http://hz.yuxming.cn/gthqdnybkj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ybcxt.top/gtvsuwwauk.html

[R47] sed 单行替换
来源：http://hz.jqgufenzy.top/gtijswacwn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuxming.cn/gtcfltukjh.html

[R48] awk 取指定列
来源：http://hz.9152youxi.cn/gtdfdesdst.html

awk '{print $1, $3}' a.txt
来源：http://hz.andypj.xyz/gtzgrivxym.html

[R49] awk 带条件
来源：http://hz.jqgufenzy.top/gtboxevazz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.316326.xyz/gtccegnhgy.html

[R50] awk 求和
来源：http://hz.9152youxi.cn/gtavnuepvm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hongshengwenyu.top/gtugwzxwje.html

[R51] 排序去重取前几
来源：http://hz.mhx1999.top/gtoevequjj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yongpay.top/gtqifziymq.html

[R52] 统计行数
来源：http://hz.dianchejie.cn/gtddfispua.html

wc -l a.txt
来源：http://hz.sysykeji.top/gtdggsxlps.html

[R53] 查看文件头与实时尾
来源：http://hz.dianchejie.cn/gtiwyifpmy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jlsjyb.cn/gtpdtdqiih.html

[R54] 比较两个文件
来源：http://hz.wangshuangyany.cn/gtsrhtvvzt.html

diff a.txt b.txt
来源：http://hz.jqgfzy.top/gtalysgglu.html

[R55] 压缩与解压
来源：http://hz.daxiang520.top/gtivomdapf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dianchejie.cn/gtpqgufslj.html

[R56] 远程拷贝
来源：http://hz.zhoulong.xyz/gtxmogbrdg.html

scp file user@host:/path/
来源：http://hz.wangdashe.top/gtjcyutdma.html

[R57] 远程执行命令
来源：http://hz.pycfn.com/gtljgkyafi.html

ssh user@host 'uptime'
来源：http://hz.zhengqikj.top/gtqdhpkikf.html

[R58] 下载文件
来源：http://hz.gzhubu.top/gtjivospau.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.52xcode.cn/gtwlstqktz.html

[R59] 发 POST JSON
来源：http://hz.xziqi.cn/gtgjnniyie.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.daxiang520.top/gttbvycuph.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhaomingkeji.xyz/gtevskngkd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.meibo888.top/gtzkwthnjh.html

[R61] 磁盘占用
来源：http://hz.cheryme.top/gttbxdqnmd.html

df -h;  du -sh *
来源：http://hz.zhiwuduotai.top/gtdkslmzfw.html

[R62] 找最占空间的文件
来源：http://hz.andypj.xyz/gtveavfepl.html

du -ah . | sort -rh | head -10
来源：http://hz.shuidangran.top/gtknbjvknk.html

[R63] 内存与进程
来源：http://hz.cqqwz.cn/gtyrmfluoc.html

free -h;  ps aux | grep nginx
来源：http://hz.xuanzx.com/gtslvkmopn.html

[R64] 结束进程
来源：http://hz.yj202588.top/gtojhgjret.html

kill -9 $(pgrep -f app.py)
来源：http://hz.svipenyu.cn/gtzxjoupct.html

[R65] 查看端口占用
来源：http://hz.nwbrower.top/gtfhykpjif.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.feifeiyinyue.top/gtfwlnjofq.html

[R66] 定时任务
来源：http://hz.shzxlz.cn/gtriliinlg.html

crontab -e;  crontab -l
来源：http://hz.9152youxi.cn/gtnnqqosxf.html

[R67] 生成随机十六进制串
来源：http://hz.bjfxy.top/gtvdeliufy.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gtloyouvkb.html

[R68] 计算文件校验值
来源：http://hz.ydzc1.top/gtijlfcqnx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daxiang520.top/gtafxzemyz.html

[R69] 生成随机密码
来源：http://hz.zhiwuduotai.top/gtfzqgnqdc.html

head -c 16 /dev/urandom | base64
来源：http://hz.pycfn.com/gtaddqlchj.html

[R70] 时间戳与互转
来源：http://hz.xingfuxueyuan.xyz/gtztgwjohs.html

date +%s;  date -d @1700000000
来源：http://hz.fengsongda.top/gtdyzgcxls.html

[R71] 日期格式化
来源：http://hz.zdqjudy.top/gtnersejyb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tianlin.xyz/gtiaselhxr.html

[R72] 等待端口就绪
来源：http://hz.hnqzz.top/gtnyfpsieq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.bjfxy.top/gtvrvsukyl.html

[R73] 分割大日志
来源：http://hz.jianghu66.top/gtbxukxixv.html

split -l 1000 big.log part_
来源：http://hz.yj20258888.top/gtfkrnxudu.html

[R74] 批量重命名
来源：http://hz.hywenlv.cn/gtsiszpdvd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.mhx1999.top/gtmjxdbneo.html

[R75] 导出环境变量
来源：http://hz.iojbl.cn/gtbajazrlx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhijiandao.cn/gtgdxgjake.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gthluwhkjt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtxbvuravw.html

[R77] 读取用户输入
来源：http://hz.sysykeji.top/gtsegaoeld.html

read -rp "请输入: " ans
来源：http://hz.ybcxt.top/gtbatjjtbx.html

[R78] 交互式菜单
来源：http://hz.cdnleiting.top/gtzyhcxguk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.kuanghao11.cn/gtenioriac.html

[R79] 解析命令行选项
来源：http://hz.bjfxy.top/gtdsayjwld.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cqqwz.cn/gtyomtpvga.html

[R80] 查看脚本执行耗时
来源：http://hz.jianghu66.top/gtqwefdxhg.html

time ./run.sh
来源：http://hz.cheryme.top/gtwroukvcc.html

================================================================================
来源：http://hz.zycfv.cn/gtjoemzbod.html

S. C / C++ 专题
来源：http://hz.zhijiandao.cn/gtydlceulb.html

================================================================================
来源：http://hz.0kj1m.cn/gtmhbkrcls.html

[S01] C：Hello World
来源：http://hz.quarkkingdee.top/gthkfyhqpr.html

#include <stdio.h>
来源：http://hz.xuanzx.com/gtquysibaw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hysaishi.cn/gtzylleski.html

[S02] C：变量与格式化输出
来源：http://hz.nanxuanxn.top/gtajqnbbno.html

int a = 10; printf("%d\n", a);
来源：http://hz.shuidangran.top/gtvnspnfuk.html

[S03] C：读入整数
来源：http://hz.jinghuilouyu.cn/gthvpewhra.html

int x; scanf("%d", &x);
来源：http://hz.chenzaomai.com/gtrmmccsek.html

[S04] C：字符串复制
来源：http://hz.yongpay.top/gtkhudjlxt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.meibo888.top/gtlqefsqdo.html

[S05] C：字符串长度
来源：http://hz.zdqjudy.top/gtrjsnvfap.html

strlen(s)
来源：http://hz.haohaochexian.top/gtwyuthbrl.html

[S06] C：字符串比较
来源：http://hz.vqdsnc.cn/gtcmjpkpkm.html

strcmp(a, b) == 0
来源：http://hz.hnqzz.top/gtauwvoavb.html

[S07] C：数组遍历求和
来源：http://hz.shzxlz.cn/gtwrvsvybw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ywan-chungtsiang.top/gtbqvobztn.html

[S08] C：动态内存分配与释放
来源：http://hz.yueranfly.top/gtpwzrukvu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cucudq.cn/gtudasohpu.html

[S09] C：结构体定义与初始化
来源：http://hz.yvedp.cn/gtcrpcjcao.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tian-w.cn/gthmtxjqbw.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtsghqleic.html

int *p = &a;  *p = 5;
来源：http://hz.cashguo.top/gtyfaveofl.html

[S11] C：逐行读文件
来源：http://hz.meibo888.top/gticjnatuh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydzc1.top/gtwwmgddia.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinghuilouyu.cn/gtbdblbgje.html

fclose(f);
来源：http://hz.feifeiyinyue.top/gtwgpdforo.html

[S12] C：写文件
来源：http://hz.yuxming.cn/gtcfqiukhz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.birdmap.top/gtwpnrbqsw.html

[S13] C：宏定义
来源：http://hz.yongpay.top/gtqfnnwhyr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xuetiantiany.cn/gtjhwfqzdh.html

[S14] C：枚举
来源：http://hz.shanyushiyangtech.top/gtkfwmupko.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.0kj1m.cn/gtfmpeoggb.html

[S15] C：类型转换
来源：http://hz.jinqigufen.top/gtencpispq.html

(double) a / b
来源：http://hz.ydjk.org.cn/gtbsbicpqa.html

[S16] C：位操作置位
来源：http://hz.havefunace.top/gtjwmlhtam.html

x |= (1 << 3);
来源：http://hz.ybcxt.top/gtiebtabou.html

[S17] C：安全拼接字符串
来源：http://hz.jianghu66.top/gtwejcvffg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenlongwang.top/gtcafpbnvg.html

[S18] C：命令行参数
来源：http://hz.gaohongyu789.top/gthdtiyohs.html

int main(int argc, char **argv)
来源：http://hz.dianchejie.cn/gtfkhxufjh.html

[S19] C：快速排序
来源：http://hz.zhixingplan.top/gtqwztkugw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gtswdoqpbk.html

[S20] C：二分查找
来源：http://hz.xuetiantiany.cn/gtdagidonc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhoulong.xyz/gtlsyjfsxu.html

[S21] C：字符类别判断
来源：http://hz.hnxiangtu.top/gtvriojqae.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.redwolf501.top/gtihxnsdtv.html

[S22] C：字符串转数字
来源：http://hz.xingfuxueyuan.xyz/gtygwixuln.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xziqi.cn/gtgylrmfci.html

[S23] C：随机数
来源：http://hz.sxryk.cn/gtyzkikhrh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yonumen.top/gtgsboligo.html

[S24] C：获取本地时间
来源：http://hz.zhoulong.xyz/gtluphbnad.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ehwqpu.com/gtleigmhxv.html

[S25] C：内存拷贝
来源：http://hz.zhijiandao.cn/gtvaopfnwt.html

memcpy(dst, src, n);
来源：http://hz.yueranfly.top/gtyxvwvaln.html

[S26] C：内存清零
来源：http://hz.ybcxt.top/gtgwwesali.html

memset(a, 0, sizeof a);
来源：http://hz.sweek.top/gtthyccmsh.html

[S27] C：定义常量
来源：http://hz.feifeiyinyue.top/gturibmtfp.html

const double PI = 3.14159;
来源：http://hz.tian-w.cn/gtxrwyrnhr.html

[S28] C：静态变量
来源：http://hz.quarkkingdee.top/gteyetsdrv.html

static int counter = 0;
来源：http://hz.hysaishi.cn/gtwylqkeif.html

[S29] C：变参函数
来源：http://hz.ehwqpu.com/gthigabisr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangkeji.top/gtvntonbip.html

[S30] C：头文件保护
来源：http://hz.feifeiyinyue.top/gtjcoojmge.html

#ifndef X_H
来源：http://hz.hnxiangtu.top/gtasmtmzww.html

#define X_H
来源：http://hz.wangshuangyany.cn/gtdpnlkntf.html

#endif
来源：http://hz.sufxvd.cn/gtsnsjjwlk.html

[S31] C++：Hello World
来源：http://hz.sweek.top/gtchpqmkli.html

#include <iostream>
来源：http://hz.wangdashe.top/gtvpxabzmj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.nwbrower.top/gtezhchidn.html

[S32] C++：字符串
来源：http://hz.sysykeji.top/gtyuuqjukp.html

std::string s = "hi";  s += "!";
来源：http://hz.jlsjyb.cn/gtalenqcqz.html

[S33] C++：vector 增删
来源：http://hz.zhongyouzk.top/gtbovdibpf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuxming.cn/gtbmnxcevp.html

[S34] C++：遍历 vector
来源：http://hz.zhiwuduotai.top/gtiuwsvvff.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj202588.top/gtuyezdfvu.html

[S35] C++：map
来源：http://hz.jiagoushi.top/gtqbndxbmq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtqyugaaxb.html

[S36] C++：unordered_map
来源：http://hz.nanxinkj.top/gtzgafygww.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtshjvkdrh.html

[S37] C++：set
来源：http://hz.pengpengdd.cyou/gtdgknoyuy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.316326.xyz/gtsnhgknun.html

[S38] C++：排序
来源：http://hz.ppjwa.cn/gtqbmbrpiz.html

std::sort(v.begin(), v.end());
来源：http://hz.yanxiufei.cn/gtgeivuero.html

[S39] C++：自定义比较器排序
来源：http://hz.ppjwa.cn/gtbfelaxtj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhijiandao.cn/gtlcbthogk.html

[S40] C++：查找元素
来源：http://hz.zhaomingkeji.xyz/gtfyojqtom.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.snrcjt.cn/gtvppgguup.html

[S41] C++：类与构造函数
来源：http://hz.sweek.top/gthzrchgzy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenlongwang.top/gtafqqvdaz.html

[S42] C++：继承与虚函数
来源：http://hz.zycfv.cn/gtyjmwudrt.html

class B : public Base { public: void f() override {} };
来源：http://hz.guowangkeji.top/gtsuvfeahg.html


<!-- 参考信息 -->