代发 wailian999

ANALYZE TABLE users;
来源：http://hz.cqqwz.cn/gtxyicskdd.html

[Q71] 查看建表语句
来源：http://hz.jinqigufen.top/gtjcphdcuw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ywan-chungtsiang.top/gtbstzlaod.html

[Q72] 查看索引
来源：http://hz.jinghuilouyu.cn/gtkustgkrf.html

SHOW INDEX FROM users;
来源：http://hz.tianlin.xyz/gtjifsjoqf.html

[Q73] 查看表状态
来源：http://hz.jinqigufen.top/gtoaldwddu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sxryk.cn/gtwdtsemtp.html

[Q74] 强制使用索引
来源：http://hz.iojbl.cn/gtnujzygxw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ydzc1.top/gtjglsirgp.html

[Q75] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtfefunlut.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.0kj1m.cn/gtlvktrhvv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jyoumei.cn/gtxreambfs.html

[Q76] 按天统计
来源：http://hz.wangshuangyany.cn/gtraqrgqeo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj20258888.top/gtttktgxnf.html

[Q77] 时间加减
来源：http://hz.sysykeji.top/gttkipdtrl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.bjfxy.top/gtxcdbjced.html

[Q78] 当前时间
来源：http://hz.shanyushiyangtech.top/gtdpfeodgg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yangfankeji.com/gtyjgknvuf.html

[Q79] 字符串拼接
来源：http://hz.ppjwa.cn/gtsvlkrjcq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.feifeiyinyue.top/gtteoifjwp.html

[Q80] 字符串截取
来源：http://hz.birdmap.top/gtzkjunqxl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cdnleiting.top/gtcsafdmpu.html

[Q81] 字符串替换
来源：http://hz.ybcxt.top/gtcboxkvru.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ehwqpu.com/gtguhxface.html

[Q82] 字符长度与字节长度
来源：http://hz.redwolf501.top/gtbzcdcxpz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gtcqegngvv.html

[Q83] 大小写转换
来源：http://hz.0kj1m.cn/gtnozypukc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtsnmawxwt.html

[Q84] 去除首尾空格
来源：http://hz.daxiang520.top/gtqvlfzeym.html

SELECT TRIM(name) FROM users;
来源：http://hz.hfpthk.cn/gtdaegyuqz.html

[Q85] 数值取整
来源：http://hz.haohaochexian.top/gtysnsipal.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.meibo888.top/gtnenerswp.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtdqlatofw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhengqikj.top/gtpwqznhbh.html

[Q87] JSON 字段做条件
来源：http://hz.0kj1m.cn/gtptzmtcnk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pycfn.com/gtgxpmmaxe.html

[Q88] 行转列（条件聚合）
来源：http://hz.gaohongyu789.top/gtdwubkqgh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhiwuduotai.top/gtfxzfpmgr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhongyouzk.top/gtmncwjgdr.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangkeji.top/gtwzmlngay.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydzc1.top/gtixbbrjdq.html

[Q90] 生成序号列
来源：http://hz.andypj.xyz/gtxgkmhnmx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.52xcode.cn/gteanrtnll.html

================================================================================
来源：http://hz.ydjk.org.cn/gtlopkvfoo.html

R. Bash 专题
来源：http://hz.zhaomingkeji.xyz/gttytrxlfa.html

================================================================================
来源：http://hz.cucudq.cn/gtzphcspdi.html

[R01] shebang 与严格模式
来源：http://hz.fzhhl.top/gtoltorpup.html

#!/usr/bin/env bash
来源：http://hz.dianchejie.cn/gtdmanqdfc.html

set -euo pipefail
来源：http://hz.redwolf501.top/gtqwafdmbl.html

[R02] 变量赋值与使用
来源：http://hz.zhaomingkeji.xyz/gtehzqdtze.html

name="Tom"; echo "$name"
来源：http://hz.vqdsnc.cn/gtzracjqns.html

[R03] 只读变量
来源：http://hz.316326.xyz/gthvbojqer.html

readonly PI=3.14
来源：http://hz.cashguo.top/gtdrmeqxuz.html

[R04] 位置参数
来源：http://hz.xuetiantiany.cn/gtciweiugf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258888.top/gttwmhmwcw.html

[R05] 参数默认值
来源：http://hz.jinqigfzy.top/gthgcwykaf.html

name="${1:-default}"
来源：http://hz.cashguo.top/gtmpxpohci.html

[R06] 判断命令是否存在
来源：http://hz.svipenyu.cn/gteilxojbt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258.top/gtcvjlpgpy.html

[R07] if 判断文件
来源：http://hz.gzhubu.top/gteypgznts.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenzaomai.com/gtrzeeeqas.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gtjrrxghuf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigufen.top/gtsufwfusn.html

[R09] 字符串比较
来源：http://hz.jqgufenzy.top/gtalhjqlcd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yvedp.cn/gtlhvfzlje.html

[R10] 正则匹配
来源：http://hz.yj20258888.top/gtvlmcnlxs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.svipenyu.cn/gtdjdsjzqi.html

[R11] case 多分支
来源：http://hz.gzhubu.top/gtxgrwrzui.html

case "$1" in
来源：http://hz.hfpthk.cn/gtalfbrebb.html

start) echo "启动" ;;
来源：http://hz.hywenlv.cn/gttkwbifjk.html

stop)  echo "停止" ;;
来源：http://hz.jqgufenzy.top/gtxdblhmri.html

*)     echo "未知命令" ;;
来源：http://hz.yangfankeji.com/gtugbabkwt.html

esac
来源：http://hz.svipenyu.cn/gtoezhjlxv.html

[R12] for 遍历文件
来源：http://hz.redwolf501.top/gtimywtdio.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhaomingkeji.xyz/gtlljwculd.html

[R13] for 计数循环
来源：http://hz.chenjidiqi.icu/gtbfoobhdv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenzaomai.com/gtnrdazbjo.html

[R14] C 风格 for
来源：http://hz.sweek.top/gtsntjmmpj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258.top/gttgsljfbv.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtrwkwxaup.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhoulong.xyz/gtmupzcmyx.html

[R16] until 等待条件
来源：http://hz.mhx1999.top/gtfihnhbot.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yonumen.top/gtoasbazhj.html

[R17] 数组定义与取值
来源：http://hz.meibo888.top/gtughiwoqb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sysykeji.top/gtcgoxxskm.html

[R18] 遍历数组
来源：http://hz.yj202588.top/gtakyryzja.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ehwqpu.com/gtkddwacgy.html

[R19] 数组长度
来源：http://hz.yuanzhike.top/gtiehsjbrv.html

echo "${#arr[@]}"
来源：http://hz.xinyue.icu/gtvcdntrwa.html

[R20] 关联数组（字典）
来源：http://hz.birdmap.top/gtneallyli.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangdashe.top/gtqkmyvgyr.html

[R21] 字符串长度
来源：http://hz.wangshuangyany.cn/gtzjpcmpox.html

echo "${#s}"
来源：http://hz.shzxlz.cn/gtuhpcmthv.html

[R22] 截取子串
来源：http://hz.sysykeji.top/gtoirxfpfc.html

echo "${s:0:5}"
来源：http://hz.iojbl.cn/gtrxozaxhy.html

[R23] 字符串替换
来源：http://hz.yangfankeji.com/gtwcmauqsc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnqzz.top/gtquipvbdc.html

[R24] 大小写转换
来源：http://hz.tanke756.top/gttifhkzkn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gtsiqrzysp.html

[R25] 去后缀 / 去前缀
来源：http://hz.aibaodan.cn/gtulshnprx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenzaomai.com/gtyivmimvt.html

[R26] 命令替换
来源：http://hz.yvedp.cn/gtgdsklkar.html

now=$(date +%F); echo "$now"
来源：http://hz.tian-w.cn/gtaqjwjsog.html

[R27] 算术展开
来源：http://hz.tanke756.top/gtdeuxggpo.html

echo $((1 + 2 * 3))
来源：http://hz.jinyuanbaomall.cn/gtkcbytzph.html

[R28] 浮点运算
来源：http://hz.zhijiandao.cn/gtdkxvecla.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gtklbzmcsl.html

[R29] 定义函数
来源：http://hz.andypj.xyz/gtzrzhgboh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgfzy.top/gtxxvaiima.html

[R30] 函数返回状态码
来源：http://hz.yonumen.top/gtygerslpi.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daria6918.cn/gtxhmntjbe.html

[R31] 局部变量
来源：http://hz.sweek.top/gtbzxjoywn.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuxming.cn/gtoiyyihhy.html

[R32] 参数个数校验
来源：http://hz.tian-w.cn/gtviplymfw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhoulong.xyz/gtrmoaxyul.html

[R33] 捕获错误并提示行号
来源：http://hz.ydjk.org.cn/gtmdobinmk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hywenlv.cn/gtrklbjnbu.html

[R34] 退出时清理
来源：http://hz.jlsjyb.cn/gtapbibtbf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtolpvqnto.html

[R35] 后台执行并等待
来源：http://hz.xinyue.icu/gthznozphc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guannengcc.top/gtgmbuwmfe.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangkeji.top/gtzbgvylub.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gzhubu.top/gtekpztoag.html

[R37] 把输出赋给变量
来源：http://hz.gotoacloud.top/gtpamgihqr.html

files=$(ls -1)
来源：http://hz.c1oappe.top/gtjcxhrsle.html

[R38] 管道串联
来源：http://hz.zycfv.cn/gtvrsdkzmw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aizwys.cn/gtsoasytmn.html

[R39] 重定向标准输出与错误
来源：http://hz.guowangkeji.top/gtistqbrvw.html

cmd > out.log 2>&1
来源：http://hz.vqdsnc.cn/gtceboqohq.html

[R40] 追加写日志
来源：http://hz.hywenlv.cn/gthoxzwema.html

echo "log" >> out.log
来源：http://hz.hfpthk.cn/gtxthjzqww.html

[R41] 丢弃输出
来源：http://hz.yonumen.top/gtvsqujbay.html

cmd >/dev/null 2>&1
来源：http://hz.sxryk.cn/gtskevyquk.html

[R42] 输入重定向
来源：http://hz.fzhhl.top/gtrdyaaizb.html

wc -l < a.txt
来源：http://hz.meibo888.top/gtnoysjndf.html

[R43] 按名字查找文件
来源：http://hz.quarkkingdee.top/gtooopjtuj.html

find . -name "*.log" -type f
来源：http://hz.ydjk.org.cn/gtuoukbzyy.html

[R44] 按修改时间查找
来源：http://hz.hammf.cn/gtbzdjkkji.html

find . -mtime -7 -type f
来源：http://hz.zycfv.cn/gtteuzfyln.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtegdkvttt.html

find . -name "*.tmp" -delete
来源：http://hz.cucudq.cn/gtrcrjgtaf.html

[R46] 递归替换文件内容
来源：http://hz.gotoacloud.top/gtdlaigxxk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhaomingkeji.xyz/gtwdcresxh.html

[R47] sed 单行替换
来源：http://hz.sysykeji.top/gtttcdyece.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ppjwa.cn/gtfiplkrbj.html

[R48] awk 取指定列
来源：http://hz.9152youxi.cn/gtsesjsuux.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigfzy.top/gtofhfcnpy.html

[R49] awk 带条件
来源：http://hz.hysaishi.cn/gtbetjfrmq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxuanxn.top/gtvqcvmkuh.html

[R50] awk 求和
来源：http://hz.ydzc1.top/gtspbmswtu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yueranfly.top/gtffuepllq.html

[R51] 排序去重取前几
来源：http://hz.hongshengwenyu.top/gttxnjxkns.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guowangkeji.top/gtxxwuyvth.html

[R52] 统计行数
来源：http://hz.cdnleiting.top/gtzzbhnzkn.html

wc -l a.txt
来源：http://hz.hfpthk.cn/gtvkfdnvmw.html

[R53] 查看文件头与实时尾
来源：http://hz.gogol.net.cn/gtrxsgjtch.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.birdmap.top/gtvobqbjnb.html

[R54] 比较两个文件
来源：http://hz.52xcode.cn/gtnkoghbtn.html

diff a.txt b.txt
来源：http://hz.smart0.xyz/gtixurpxxy.html

[R55] 压缩与解压
来源：http://hz.gaohongyu789.top/gtsxjwmqax.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhixingplan.top/gtjrjarocq.html

[R56] 远程拷贝
来源：http://hz.hnxiangtu.top/gtllmpmctn.html

scp file user@host:/path/
来源：http://hz.shangyingyoupin.top/gtwvagxurr.html

[R57] 远程执行命令
来源：http://hz.ybcxt.top/gtnjlnbcpi.html

ssh user@host 'uptime'
来源：http://hz.xuetiantiany.cn/gteeemstxq.html

[R58] 下载文件
来源：http://hz.0kj1m.cn/gttdpcpovh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gthrlksnhg.html

[R59] 发 POST JSON
来源：http://hz.jinghuilouyu.cn/gtahyluixu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.fzhhl.top/gtuwkwxwva.html

[R60] 只看 HTTP 状态码
来源：http://hz.fengsongda.top/gtamudocsy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tianlin.xyz/gtyyaiitaf.html

[R61] 磁盘占用
来源：http://hz.hfpthk.cn/gtxriernxt.html

df -h;  du -sh *
来源：http://hz.hnqzz.top/gtqixmfozm.html

[R62] 找最占空间的文件
来源：http://hz.chenlongwang.top/gtjsxvjdin.html

du -ah . | sort -rh | head -10
来源：http://hz.zhaomingkeji.xyz/gtaunyembx.html

[R63] 内存与进程
来源：http://hz.bjfxy.top/gtxehutvxm.html

free -h;  ps aux | grep nginx
来源：http://hz.daxiang520.top/gttptuytod.html

[R64] 结束进程
来源：http://hz.shangyingyoupin.top/gtmbrxvyen.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hywenlv.cn/gtklrgnxzk.html

[R65] 查看端口占用
来源：http://hz.jinqigufen.top/gtlgfbohrk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cqqwz.cn/gtkprgcwyq.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtekfradon.html

crontab -e;  crontab -l
来源：http://hz.xuanzx.com/gtgsyahbcm.html

[R67] 生成随机十六进制串
来源：http://hz.yuanzhike.top/gtufylokvn.html

openssl rand -hex 16
来源：http://hz.zhongyouzk.top/gtxruqfygt.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangtech.top/gtrnmddwri.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangkeji.top/gtrbvdszgl.html

[R69] 生成随机密码
来源：http://hz.xinyue.icu/gtzpomvmco.html

head -c 16 /dev/urandom | base64
来源：http://hz.xuetiantiany.cn/gtjwazvmla.html

[R70] 时间戳与互转
来源：http://hz.chenlongwang.top/gthbrjmczp.html

date +%s;  date -d @1700000000
来源：http://hz.0kj1m.cn/gttkgretkg.html

[R71] 日期格式化
来源：http://hz.daria6918.cn/gtiempamtt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pycfn.com/gticszhttx.html

[R72] 等待端口就绪
来源：http://hz.nwbrower.top/gtqsfncznj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj20258888.top/gtvoloorww.html

[R73] 分割大日志
来源：http://hz.sweek.top/gtmcryiffl.html

split -l 1000 big.log part_
来源：http://hz.yangfankeji.com/gtrsgmpttj.html

[R74] 批量重命名
来源：http://hz.nanxuanxn.top/gtbhktvhrn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cqqwz.cn/gtpnvnvscq.html

[R75] 导出环境变量
来源：http://hz.havefunace.top/gtykqmxxmx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhoulong.xyz/gtwftbdxpd.html

[R76] 使用临时文件
来源：http://hz.316326.xyz/gtmgnsvftn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtsnlzuwkr.html

[R77] 读取用户输入
来源：http://hz.cucudq.cn/gtldqdlfuo.html

read -rp "请输入: " ans
来源：http://hz.shzxlz.cn/gtjqjesygr.html

[R78] 交互式菜单
来源：http://hz.c1oappe.top/gttpefsoxe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.iojbl.cn/gtqwxqqtpq.html

[R79] 解析命令行选项
来源：http://hz.hnxiangtu.top/gtpidmfzms.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zdqjudy.top/gtecoeuryd.html

[R80] 查看脚本执行耗时
来源：http://hz.aibaodan.cn/gtuceszzex.html

time ./run.sh
来源：http://hz.svipenyu.cn/gtrzfqtsga.html

================================================================================
来源：http://hz.sweek.top/gtimbwesaq.html

S. C / C++ 专题
来源：http://hz.jinghuilouyu.cn/gtybezyrpm.html

================================================================================
来源：http://hz.birdmap.top/gtbidinmdm.html

[S01] C：Hello World
来源：http://hz.kuanghao11.cn/gttewdfqgz.html

#include <stdio.h>
来源：http://hz.hongshengwenyu.top/gtitqrvepz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zycfv.cn/gtnaajseux.html

[S02] C：变量与格式化输出
来源：http://hz.jlsjyb.cn/gtygcpabjc.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenjidiqi.icu/gtenfvmgny.html

[S03] C：读入整数
来源：http://hz.chenlongwang.top/gtaksomwoa.html

int x; scanf("%d", &x);
来源：http://hz.ybcxt.top/gtulbybiqv.html

[S04] C：字符串复制
来源：http://hz.xziqi.cn/gtaocbcicn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zdqjudy.top/gtlzanzyoe.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtyqdopnts.html

strlen(s)
来源：http://hz.0kj1m.cn/gtqooqmtlj.html

[S06] C：字符串比较
来源：http://hz.hongshengwenyu.top/gtpsmubgdh.html

strcmp(a, b) == 0
来源：http://hz.c1oappe.top/gtdnblieiq.html

[S07] C：数组遍历求和
来源：http://hz.iojbl.cn/gtpmdxsqts.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.smart0.xyz/gtmenyzppk.html

[S08] C：动态内存分配与释放
来源：http://hz.yj202588.top/gtdanfgyjq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guowangkeji.top/gthpkllfss.html

[S09] C：结构体定义与初始化
来源：http://hz.xylfe.cn/gtnjycmbnu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gaohongyu789.top/gtoetdgxwj.html

[S10] C：指针与解引用
来源：http://hz.chenjidiqi.icu/gtbeyauaoe.html

int *p = &a;  *p = 5;
来源：http://hz.yj202588.top/gtqtcoghqn.html

[S11] C：逐行读文件
来源：http://hz.wangshuangyany.cn/gtfsopjwrl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dianchejie.cn/gtmmlscmcu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.daxiang520.top/gtwkmxtkxl.html

fclose(f);
来源：http://hz.andypj.xyz/gtbkouqsjg.html

[S12] C：写文件
来源：http://hz.tian-w.cn/gtvnplzazm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.kuanghao11.cn/gtcddhzztz.html

[S13] C：宏定义
来源：http://hz.quarkkingdee.top/gtaodfnehf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daxiang520.top/gtmuponckn.html

[S14] C：枚举
来源：http://hz.ivvv.top/gtcmbmngsk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jianghu66.top/gtprvtkzyp.html

[S15] C：类型转换
来源：http://hz.9152youxi.cn/gtjlnbbrqm.html

(double) a / b
来源：http://hz.zdqjudy.top/gtuoncslks.html

[S16] C：位操作置位
来源：http://hz.zhongyouzk.top/gtsowfkvfd.html

x |= (1 << 3);
来源：http://hz.xziqi.cn/gtrcmqoxal.html

[S17] C：安全拼接字符串
来源：http://hz.yuanzhike.top/gtlkciixgq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xylfe.cn/gturqkbpjj.html

[S18] C：命令行参数
来源：http://hz.hfpthk.cn/gtsdbnvhrk.html

int main(int argc, char **argv)
来源：http://hz.zdqjudy.top/gttzwtgzih.html

[S19] C：快速排序
来源：http://hz.xingfuxueyuan.xyz/gtrjfjvbbg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtidokczbo.html

[S20] C：二分查找
来源：http://hz.yanxiufei.cn/gtcahizwdz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cheryme.top/gtzljijtpv.html

[S21] C：字符类别判断
来源：http://hz.xuanzx.com/gtsbtjpiaa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhijiandao.cn/gtpypxnbno.html

[S22] C：字符串转数字
来源：http://hz.tianlin.xyz/gtmqwjteez.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hysaishi.cn/gttijzcoef.html

[S23] C：随机数
来源：http://hz.hywenlv.cn/gtlrklpqvh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhoulong.xyz/gtrqtqishv.html

[S24] C：获取本地时间
来源：http://hz.jinghuilouyu.cn/gtcvbhwzcv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuanzhike.top/gtaczmqdxs.html

[S25] C：内存拷贝
来源：http://hz.zhixingplan.top/gtzbaevltl.html

memcpy(dst, src, n);
来源：http://hz.jiagoushi.top/gtmatajnsf.html

[S26] C：内存清零
来源：http://hz.ppjwa.cn/gtedyhjigt.html

memset(a, 0, sizeof a);
来源：http://hz.nwbrower.top/gtkivlbulu.html

[S27] C：定义常量
来源：http://hz.jinqigfzy.top/gtqjevuegj.html

const double PI = 3.14159;
来源：http://hz.jiagoushi.top/gtujtlivjh.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gtstlvzekn.html

static int counter = 0;
来源：http://hz.zhongyouzk.top/gtlfcyfoqb.html

[S29] C：变参函数
来源：http://hz.guannengcc.top/gthweqbszj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.mhx1999.top/gtmvotldsj.html

[S30] C：头文件保护
来源：http://hz.tanke756.top/gtuhlxszgj.html

#ifndef X_H
来源：http://hz.shanyushiyangtech.top/gtutslflcw.html

#define X_H
来源：http://hz.shanyushiyangtech.top/gtljpggxlf.html

#endif
来源：http://hz.havefunace.top/gtgaxwdmua.html

[S31] C++：Hello World
来源：http://hz.hysaishi.cn/gtgdpeooxk.html

#include <iostream>
来源：http://hz.cashguo.top/gtjtqcmajc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangshuangyany.cn/gtnpszueoh.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtfkiuagkb.html

std::string s = "hi";  s += "!";
来源：http://hz.zycfv.cn/gtzsbuitli.html

[S33] C++：vector 增删
来源：http://hz.yj20258.top/gtnbameruc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pengpengdd.cyou/gtfnrqpifv.html

[S34] C++：遍历 vector
来源：http://hz.dianchejie.cn/gtblwuuexk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenzaomai.com/gtojlnjwfq.html

[S35] C++：map
来源：http://hz.zhixingplan.top/gtlsrjjwys.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtyrikrrft.html

[S36] C++：unordered_map
来源：http://hz.haohaochexian.top/gtfkgswcpp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtovbvehuz.html

[S37] C++：set
来源：http://hz.aizwys.cn/gtcxmmihol.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.9152youxi.cn/gtlsguwbly.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtzfjcpdtt.html

std::sort(v.begin(), v.end());
来源：http://hz.gzhubu.top/gtposgzwxg.html

[S39] C++：自定义比较器排序
来源：http://hz.jinyuanbaomall.cn/gtgrdxanes.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxinkj.top/gtgpvtpqpl.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtnjyanrol.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jyoumei.cn/gtqawqqlvq.html


<!-- 参考信息 -->