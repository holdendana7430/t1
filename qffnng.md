代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.chenjidiqi.icu/gtevxgcuyd.html

[Q60] 取上一行 / 下一行
来源：http://hz.dashuyun.cn/gtxstvzzlw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gtouknalcs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtznnsgqla.html

[Q61] 移动平均
来源：http://hz.ywan-chungtsiang.top/gtdfhswsfk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.iojbl.cn/gtmhvsjjju.html

[Q62] 分组占比
来源：http://hz.shanyushiyangkeji.top/gtuszuvhpv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtpeogqvxh.html

[Q63] 开启事务
来源：http://hz.ivvv.top/gtmskiqqcw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydzc1.top/gtbpxxolwl.html

[Q64] 提交事务
来源：http://hz.nwbrower.top/gtkaptbrfm.html

COMMIT;
来源：http://hz.xylfe.cn/gtxwfxaphs.html

[Q65] 回滚事务
来源：http://hz.yj20258.top/gtyijjnedw.html

ROLLBACK;
来源：http://hz.hfpthk.cn/gtshlbhopt.html

[Q66] 行锁查询
来源：http://hz.cdnleiting.top/gtnemknuvf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.snrcjt.cn/gtdnjynekb.html

[Q67] 设置隔离级别
来源：http://hz.yuxming.cn/gtumwsgwej.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gttxhhkgao.html

[Q68] 保存点
来源：http://hz.316326.xyz/gtqlxwjuev.html

SAVEPOINT sp1;
来源：http://hz.yvedp.cn/gtcorexorc.html

ROLLBACK TO sp1;
来源：http://hz.hongshengwenyu.top/gtmjzjngvu.html

[Q69] 查看执行计划
来源：http://hz.andypj.xyz/gtddmhxzmk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.c1oappe.top/gtveehihnx.html

[Q70] 更新统计信息
来源：http://hz.c1oappe.top/gtcaynpsqa.html

ANALYZE TABLE users;
来源：http://hz.svipenyu.cn/gtqqfxvajx.html

[Q71] 查看建表语句
来源：http://hz.ivvv.top/gtgmhevkiu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gaohongyu789.top/gtjtvejiul.html

[Q72] 查看索引
来源：http://hz.aizwys.cn/gtjwuwuutj.html

SHOW INDEX FROM users;
来源：http://hz.cqqwz.cn/gtjdbufhej.html

[Q73] 查看表状态
来源：http://hz.jqgfzy.top/gtcbgnxcdp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hfpthk.cn/gtteoicagi.html

[Q74] 强制使用索引
来源：http://hz.ydzc1.top/gtngmyzmnc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.daxiang520.top/gtbdwzyqdy.html

[Q75] 日期格式化
来源：http://hz.hammf.cn/gtulodngmm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gotoacloud.top/gtcswaxykr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sufxvd.cn/gtkechvqqk.html

[Q76] 按天统计
来源：http://hz.hysaishi.cn/gtqbxrdejq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hfpthk.cn/gtgsddxejy.html

[Q77] 时间加减
来源：http://hz.yj20258.top/gtbqjuyjhi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hammf.cn/gtvxghubvh.html

[Q78] 当前时间
来源：http://hz.sweek.top/gtluxoxikd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258888.top/gtbmvbdmxa.html

[Q79] 字符串拼接
来源：http://hz.mhx1999.top/gtfkdurgiz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pycfn.com/gtvqwvifkc.html

[Q80] 字符串截取
来源：http://hz.316326.xyz/gtvybfakyn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dianchejie.cn/gtajxkzcqm.html

[Q81] 字符串替换
来源：http://hz.hongshengwenyu.top/gtmpnjfydz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hysaishi.cn/gtqajwhlrk.html

[Q82] 字符长度与字节长度
来源：http://hz.c1oappe.top/gtomzvoxve.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yueranfly.top/gtuoohbwxb.html

[Q83] 大小写转换
来源：http://hz.jinqigfzy.top/gtruxnqloi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhijiandao.cn/gtsuppvrjr.html

[Q84] 去除首尾空格
来源：http://hz.gotoacloud.top/gtwbkznsex.html

SELECT TRIM(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtpjwlvghn.html

[Q85] 数值取整
来源：http://hz.shuidangran.top/gtdnvbdpzc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hnqzz.top/gtzetgjxfz.html

[Q86] 读取 JSON 字段
来源：http://hz.jianghu66.top/gtrhlxczzc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hywenlv.cn/gtelwxzgxf.html

[Q87] JSON 字段做条件
来源：http://hz.jinyuanbaomall.cn/gtuccuxhma.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jiagoushi.top/gtymmjytez.html

[Q88] 行转列（条件聚合）
来源：http://hz.yangfankeji.com/gtsutqndyq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gaohongyu789.top/gtvufvkfrp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtlobxuvpk.html

[Q89] 判断表是否存在
来源：http://hz.iojbl.cn/gtswxikwnl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gaohongyu789.top/gthjahfhkx.html

[Q90] 生成序号列
来源：http://hz.tanke756.top/gtyryghxpk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cheryme.top/gtgpzywmdo.html

================================================================================
来源：http://hz.ydjk.org.cn/gtowgsouyi.html

R. Bash 专题
来源：http://hz.aibaodan.cn/gtnblcnlba.html

================================================================================
来源：http://hz.cheryme.top/gtipruzaqy.html

[R01] shebang 与严格模式
来源：http://hz.ivvv.top/gtmodxhiie.html

#!/usr/bin/env bash
来源：http://hz.tian-w.cn/gtuhibzbgb.html

set -euo pipefail
来源：http://hz.zdqjudy.top/gtmjuaehpc.html

[R02] 变量赋值与使用
来源：http://hz.zdqjudy.top/gtgcwclewl.html

name="Tom"; echo "$name"
来源：http://hz.nanxinkj.top/gtnzndkjfq.html

[R03] 只读变量
来源：http://hz.sxryk.cn/gtfljtluyc.html

readonly PI=3.14
来源：http://hz.ppjwa.cn/gtbgxwkqyx.html

[R04] 位置参数
来源：http://hz.zhaomingkeji.xyz/gtasxkbuhq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shangyingyoupin.top/gtanscsslw.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtthunuira.html

name="${1:-default}"
来源：http://hz.yangfankeji.com/gtrvwbcdoz.html

[R06] 判断命令是否存在
来源：http://hz.kuanghao11.cn/gtcigfydcn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hammf.cn/gtikbhdmjd.html

[R07] if 判断文件
来源：http://hz.shanyushiyangtech.top/gtaalfnvhk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj20258888.top/gtdbcbnula.html

[R08] 数值比较
来源：http://hz.tanke756.top/gtqifrjzfv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.9152youxi.cn/gtgykfqevh.html

[R09] 字符串比较
来源：http://hz.hysaishi.cn/gtfgujtbet.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.smart0.xyz/gtbzzbeezq.html

[R10] 正则匹配
来源：http://hz.zhiwuduotai.top/gtbtagsmjs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cashguo.top/gtmigiexzl.html

[R11] case 多分支
来源：http://hz.zhongyouzk.top/gtzggeuhoy.html

case "$1" in
来源：http://hz.cdnleiting.top/gtmaygpslv.html

start) echo "启动" ;;
来源：http://hz.yuanzhike.top/gtxturdrwi.html

stop)  echo "停止" ;;
来源：http://hz.havefunace.top/gtmhrfnwby.html

*)     echo "未知命令" ;;
来源：http://hz.52xcode.cn/gtrojlsaft.html

esac
来源：http://hz.jinqigufen.top/gtjirxkswn.html

[R12] for 遍历文件
来源：http://hz.daria6918.cn/gtyomeefnm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yangfankeji.com/gthehjhrxx.html

[R13] for 计数循环
来源：http://hz.zhoulong.xyz/gteupvdzom.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtdouynhcn.html

[R14] C 风格 for
来源：http://hz.gaohongyu789.top/gtrdeaovok.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gthevzosyi.html

[R15] while 逐行读文件
来源：http://hz.sysykeji.top/gtzrlymwwr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tianlin.xyz/gthyflwcme.html

[R16] until 等待条件
来源：http://hz.wangdashe.top/gttqnzwfug.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gtbbxmnale.html

[R17] 数组定义与取值
来源：http://hz.jinyuanbaomall.cn/gtlaskoqte.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xingfuxueyuan.xyz/gtrmhpqvif.html

[R18] 遍历数组
来源：http://hz.jqgufenzy.top/gtpaqtkhho.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hfpthk.cn/gtvoqotcnm.html

[R19] 数组长度
来源：http://hz.gaohongyu789.top/gtnxfkectw.html

echo "${#arr[@]}"
来源：http://hz.havefunace.top/gturkfczte.html

[R20] 关联数组（字典）
来源：http://hz.ppjwa.cn/gtqhekgoiy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnxiangtu.top/gtlrqdiblm.html

[R21] 字符串长度
来源：http://hz.ydjk.org.cn/gtytiimets.html

echo "${#s}"
来源：http://hz.iojbl.cn/gtoeenvluk.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gtqgfrxtau.html

echo "${s:0:5}"
来源：http://hz.jqgufenzy.top/gtadapsmaf.html

[R23] 字符串替换
来源：http://hz.hnqzz.top/gtcntpidpm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yueranfly.top/gtncfehfyt.html

[R24] 大小写转换
来源：http://hz.ivvv.top/gthfxwrvvm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258.top/gtafamkrvi.html

[R25] 去后缀 / 去前缀
来源：http://hz.shuidangran.top/gtwknoixau.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgfzy.top/gthfnboddu.html

[R26] 命令替换
来源：http://hz.yj20258888.top/gtwqtxjgva.html

now=$(date +%F); echo "$now"
来源：http://hz.zhixingplan.top/gtxttklybh.html

[R27] 算术展开
来源：http://hz.wangdashe.top/gtjzbyqram.html

echo $((1 + 2 * 3))
来源：http://hz.wangshuangyany.cn/gtbapbswlw.html

[R28] 浮点运算
来源：http://hz.wangdashe.top/gtvzcmluus.html

echo "scale=2; 10/3" | bc
来源：http://hz.nanxinkj.top/gtzgnwtnow.html

[R29] 定义函数
来源：http://hz.yj20258.top/gtfgdupfyj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tanke756.top/gthlxfblkg.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtkagzpryp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tian-w.cn/gtmyqxyccx.html

[R31] 局部变量
来源：http://hz.jinqigufen.top/gtuvtgwroo.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuanzx.com/gthhbmhhgi.html

[R32] 参数个数校验
来源：http://hz.gotoacloud.top/gtyuhxfloh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sweek.top/gthnaatbht.html

[R33] 捕获错误并提示行号
来源：http://hz.316326.xyz/gtlkqmpwri.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.kuanghao11.cn/gticvumbjl.html

[R34] 退出时清理
来源：http://hz.hnqzz.top/gtrtedeqnf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtqkqdxqjt.html

[R35] 后台执行并等待
来源：http://hz.9152youxi.cn/gtatwddvte.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jqgufenzy.top/gtlaipbkna.html

[R36] 并发执行多个任务
来源：http://hz.aizwys.cn/gttnoyjapk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cheryme.top/gtlzkbsxwb.html

[R37] 把输出赋给变量
来源：http://hz.jlsjyb.cn/gtunmvnajy.html

files=$(ls -1)
来源：http://hz.vqdsnc.cn/gtjvxpangd.html

[R38] 管道串联
来源：http://hz.aibaodan.cn/gtgbimeccl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenjidiqi.icu/gtzztdmxtj.html

[R39] 重定向标准输出与错误
来源：http://hz.sysykeji.top/gtklbhqhig.html

cmd > out.log 2>&1
来源：http://hz.svipenyu.cn/gthgaaowoz.html

[R40] 追加写日志
来源：http://hz.xuetiantiany.cn/gtesryuawo.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtamacqgqe.html

[R41] 丢弃输出
来源：http://hz.fengsongda.top/gtecackczj.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigufen.top/gthnwendrq.html

[R42] 输入重定向
来源：http://hz.hammf.cn/gtejpirfpa.html

wc -l < a.txt
来源：http://hz.feifeiyinyue.top/gtfejbsuwq.html

[R43] 按名字查找文件
来源：http://hz.zhaomingkeji.xyz/gtxxpcniwp.html

find . -name "*.log" -type f
来源：http://hz.zycfv.cn/gtfmpbbbdi.html

[R44] 按修改时间查找
来源：http://hz.shuidangran.top/gtquwakwyf.html

find . -mtime -7 -type f
来源：http://hz.havefunace.top/gtuscxbzqi.html

[R45] 批量删除
来源：http://hz.shuidangran.top/gtxdnpuvif.html

find . -name "*.tmp" -delete
来源：http://hz.fzhhl.top/gtxjkpgdfk.html

[R46] 递归替换文件内容
来源：http://hz.wangdashe.top/gtgtiztktt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhiwuduotai.top/gtroogyrdf.html

[R47] sed 单行替换
来源：http://hz.hnxiangtu.top/gtshttobvr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shzxlz.cn/gtvqpenatk.html

[R48] awk 取指定列
来源：http://hz.jiagoushi.top/gtcacyfmec.html

awk '{print $1, $3}' a.txt
来源：http://hz.sxryk.cn/gtwmqteqek.html

[R49] awk 带条件
来源：http://hz.shanyushiyangkeji.top/gtpfkqrdlg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.smart0.xyz/gtqdntputn.html

[R50] awk 求和
来源：http://hz.pycfn.com/gtlbjdpeno.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nwbrower.top/gtcsjxixgb.html

[R51] 排序去重取前几
来源：http://hz.yuanzhike.top/gtlmrqqfor.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sweek.top/gtmcemfarj.html

[R52] 统计行数
来源：http://hz.pycfn.com/gtlhrobnqh.html

wc -l a.txt
来源：http://hz.shanyushiyangkeji.top/gtysbreeqd.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtkrqxliwd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pycfn.com/gtyxhqjeny.html

[R54] 比较两个文件
来源：http://hz.xingfuxueyuan.xyz/gthwkzczef.html

diff a.txt b.txt
来源：http://hz.cqqwz.cn/gtpxdrimeu.html

[R55] 压缩与解压
来源：http://hz.ivvv.top/gtzvmfobxu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cashguo.top/gtgsfebwkt.html

[R56] 远程拷贝
来源：http://hz.ybcxt.top/gtbuzreqwu.html

scp file user@host:/path/
来源：http://hz.gogol.net.cn/gteaqytbsi.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangtech.top/gtjzainivp.html

ssh user@host 'uptime'
来源：http://hz.zhengqikj.top/gtmbjjvwlz.html

[R58] 下载文件
来源：http://hz.shuidangran.top/gtdgrmorcw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pycfn.com/gtnofuiibs.html

[R59] 发 POST JSON
来源：http://hz.sxryk.cn/gtqlajgukm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pycfn.com/gtojtredoo.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgfzy.top/gtqjkqxsgu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhoulong.xyz/gtnkvoqncb.html

[R61] 磁盘占用
来源：http://hz.cdnleiting.top/gtkrwpjjwh.html

df -h;  du -sh *
来源：http://hz.svipenyu.cn/gtuydcoobb.html

[R62] 找最占空间的文件
来源：http://hz.yj20258.top/gtgnnongpv.html

du -ah . | sort -rh | head -10
来源：http://hz.birdmap.top/gtktpiohdb.html

[R63] 内存与进程
来源：http://hz.pengpengdd.cyou/gtsyxxbaiw.html

free -h;  ps aux | grep nginx
来源：http://hz.yangfankeji.com/gtrbdezemq.html

[R64] 结束进程
来源：http://hz.cucudq.cn/gtxpbgvums.html

kill -9 $(pgrep -f app.py)
来源：http://hz.aizwys.cn/gtmrxnhlct.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtdwjiadbk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.52xcode.cn/gtxbuwdzrx.html

[R66] 定时任务
来源：http://hz.jinyuanbaomall.cn/gtfnmbyyxq.html

crontab -e;  crontab -l
来源：http://hz.hywenlv.cn/gtrppfbgwa.html

[R67] 生成随机十六进制串
来源：http://hz.shanyushiyangkeji.top/gtnfmbgsyy.html

openssl rand -hex 16
来源：http://hz.fzhhl.top/gtyrnyirne.html

[R68] 计算文件校验值
来源：http://hz.kuanghao11.cn/gtpfnnowlo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydjk.org.cn/gthaetfiza.html

[R69] 生成随机密码
来源：http://hz.0kj1m.cn/gtwkcbhlkd.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangtech.top/gtbulfzgew.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtvhgixsul.html

date +%s;  date -d @1700000000
来源：http://hz.andypj.xyz/gtqfouekay.html

[R71] 日期格式化
来源：http://hz.meibo888.top/gtpecnorvp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.0kj1m.cn/gtrcirunps.html

[R72] 等待端口就绪
来源：http://hz.iojbl.cn/gtwaerbdtc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xziqi.cn/gttfougbra.html

[R73] 分割大日志
来源：http://hz.quarkkingdee.top/gtgvzmbahe.html

split -l 1000 big.log part_
来源：http://hz.jinghuilouyu.cn/gthncbfshd.html

[R74] 批量重命名
来源：http://hz.jinqigfzy.top/gtlahoaccg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.mhx1999.top/gtdndepcty.html

[R75] 导出环境变量
来源：http://hz.svipenyu.cn/gtgehuyxsu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daxiang520.top/gtiqviyfkt.html

[R76] 使用临时文件
来源：http://hz.yuanzhike.top/gtgewdquwl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtldflshzt.html

[R77] 读取用户输入
来源：http://hz.iojbl.cn/gtuseqrlxu.html

read -rp "请输入: " ans
来源：http://hz.havefunace.top/gtadysodnn.html

[R78] 交互式菜单
来源：http://hz.pengpengdd.cyou/gtjaetsflj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.snrcjt.cn/gtxdioepgj.html

[R79] 解析命令行选项
来源：http://hz.daria6918.cn/gtwljmghdu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yangfankeji.com/gtjyppnpza.html

[R80] 查看脚本执行耗时
来源：http://hz.0kj1m.cn/gtseozkrrf.html

time ./run.sh
来源：http://hz.pengpengdd.cyou/gtcxkaxbbc.html

================================================================================
来源：http://hz.chenzaomai.com/gtpgeppgkd.html

S. C / C++ 专题
来源：http://hz.hongshengwenyu.top/gtbuifpztk.html

================================================================================
来源：http://hz.cdnleiting.top/gtotrqhndr.html

[S01] C：Hello World
来源：http://hz.yonumen.top/gtuzkaqbki.html

#include <stdio.h>
来源：http://hz.hysaishi.cn/gtihjhicfe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gaohongyu789.top/gtjmajzrog.html

[S02] C：变量与格式化输出
来源：http://hz.aibaodan.cn/gtesgxhsnz.html

int a = 10; printf("%d\n", a);
来源：http://hz.pengpengdd.cyou/gtzekychsv.html

[S03] C：读入整数
来源：http://hz.ybcxt.top/gtcbybggyg.html

int x; scanf("%d", &x);
来源：http://hz.svipenyu.cn/gthsfzetoc.html

[S04] C：字符串复制
来源：http://hz.sufxvd.cn/gtqtgdodmn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhengqikj.top/gtuyhwuncz.html

[S05] C：字符串长度
来源：http://hz.9152youxi.cn/gtapcpkgoy.html

strlen(s)
来源：http://hz.shanyushiyangkeji.top/gtvcdxufov.html

[S06] C：字符串比较
来源：http://hz.cdnleiting.top/gtzireyjbr.html

strcmp(a, b) == 0
来源：http://hz.xylfe.cn/gtvsxpstgu.html

[S07] C：数组遍历求和
来源：http://hz.zhongyouzk.top/gtmxqzxfjl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xuanzx.com/gtrwqtccbl.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258.top/gtgdhuafbh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.feifeiyinyue.top/gtwirhvtkr.html

[S09] C：结构体定义与初始化
来源：http://hz.xinyue.icu/gtveciexte.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xinyue.icu/gtqdghadza.html

[S10] C：指针与解引用
来源：http://hz.aibaodan.cn/gtlgbhihrx.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigufen.top/gtjbxdrjbq.html

[S11] C：逐行读文件
来源：http://hz.zdqjudy.top/gtswbnznkk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jianghu66.top/gtgsflqiss.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxinkj.top/gtszquzxbd.html

fclose(f);
来源：http://hz.hnqzz.top/gtlwwawebo.html

[S12] C：写文件
来源：http://hz.yj20258.top/gtihdyblns.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhixingplan.top/gtvlaifgla.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtaoikfqpx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.havefunace.top/gtejfjfmbt.html

[S14] C：枚举
来源：http://hz.tianlin.xyz/gturlwadtv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.0kj1m.cn/gtanjwojah.html

[S15] C：类型转换
来源：http://hz.fengsongda.top/gtfqjbyrhc.html

(double) a / b
来源：http://hz.haohaochexian.top/gtyhegkzmi.html

[S16] C：位操作置位
来源：http://hz.hfpthk.cn/gtwvslgarc.html

x |= (1 << 3);
来源：http://hz.hongshengwenyu.top/gtpwnfnxlt.html

[S17] C：安全拼接字符串
来源：http://hz.ehwqpu.com/gtjfaklhbg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.redwolf501.top/gtykcfvepf.html

[S18] C：命令行参数
来源：http://hz.aibaodan.cn/gttguahous.html

int main(int argc, char **argv)
来源：http://hz.zdqjudy.top/gtbuncokcg.html

[S19] C：快速排序
来源：http://hz.zycfv.cn/gtfyngmufz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gthrdohyge.html

[S20] C：二分查找
来源：http://hz.xingfuxueyuan.xyz/gtzygdjtkg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtvuodlspa.html

[S21] C：字符类别判断
来源：http://hz.smart0.xyz/gtkjupbvcv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xuetiantiany.cn/gtsdlccxqz.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtvfaraiya.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydjk.org.cn/gtowjdqcfq.html

[S23] C：随机数
来源：http://hz.iojbl.cn/gtwdjhvamb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinyuanbaomall.cn/gtpyqluqbi.html

[S24] C：获取本地时间
来源：http://hz.snrcjt.cn/gtakzxhzlw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gaohongyu789.top/gtcqajpyrz.html

[S25] C：内存拷贝
来源：http://hz.guannengcc.top/gtnqqwcikh.html

memcpy(dst, src, n);
来源：http://hz.iojbl.cn/gtuozouyyf.html

[S26] C：内存清零
来源：http://hz.smart0.xyz/gtzwppczyz.html

memset(a, 0, sizeof a);
来源：http://hz.tianlin.xyz/gtlbfglkia.html

[S27] C：定义常量
来源：http://hz.pycfn.com/gtjlemnajw.html

const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtmuogfnxq.html

[S28] C：静态变量
来源：http://hz.svipenyu.cn/gtckdpznxp.html

static int counter = 0;
来源：http://hz.birdmap.top/gtfhmpgvpt.html

[S29] C：变参函数
来源：http://hz.ybcxt.top/gtiwsopwjk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.havefunace.top/gtyjxzoozb.html

[S30] C：头文件保护
来源：http://hz.gotoacloud.top/gtoqfqkkag.html


<!-- 参考信息 -->