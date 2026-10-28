代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aizwys.cn/gtxsofnkjt.html

[Q58] 累计求和
来源：http://hz.hnqzz.top/gtjewnkoyp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xziqi.cn/gtulxmvyor.html

[Q59] 分组内累计
来源：http://hz.yanxiufei.cn/gtgyctamww.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.bjfxy.top/gtkhhmhkma.html

[Q60] 取上一行 / 下一行
来源：http://hz.yueranfly.top/gtbnubbyak.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhoulong.xyz/gtgvgdrthp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hywenlv.cn/gtoctqkkzs.html

[Q61] 移动平均
来源：http://hz.xylfe.cn/gtlkcsizxp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jyoumei.cn/gtevlqurpw.html

[Q62] 分组占比
来源：http://hz.shangyingyoupin.top/gtvsvjbyxz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gttejizwju.html

[Q63] 开启事务
来源：http://hz.hfpthk.cn/gtxezohupk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yvedp.cn/gtlytgurke.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gtcctpoylz.html

COMMIT;
来源：http://hz.jianghu66.top/gtqkwibniv.html

[Q65] 回滚事务
来源：http://hz.52xcode.cn/gtobnepmxb.html

ROLLBACK;
来源：http://hz.haohaochexian.top/gtbfiztluu.html

[Q66] 行锁查询
来源：http://hz.xuanzx.com/gtzzlnxqad.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhoulong.xyz/gtyvgtrrld.html

[Q67] 设置隔离级别
来源：http://hz.316326.xyz/gtfbrvgdbb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxinkj.top/gtbekafzhi.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtslxwadbw.html

SAVEPOINT sp1;
来源：http://hz.cheryme.top/gtcgobblik.html

ROLLBACK TO sp1;
来源：http://hz.wangdashe.top/gtcvfcmymx.html

[Q69] 查看执行计划
来源：http://hz.sweek.top/gtpjszhbzp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.vqdsnc.cn/gtqlhquwko.html

[Q70] 更新统计信息
来源：http://hz.feifeiyinyue.top/gtsievxtxw.html

ANALYZE TABLE users;
来源：http://hz.yj202588.top/gtoimbqklw.html

[Q71] 查看建表语句
来源：http://hz.cdnleiting.top/gthhqctoby.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yangfankeji.com/gtlllxtcii.html

[Q72] 查看索引
来源：http://hz.smart0.xyz/gtldvdbdir.html

SHOW INDEX FROM users;
来源：http://hz.feifeiyinyue.top/gtzqgzvnyu.html

[Q73] 查看表状态
来源：http://hz.shuidangran.top/gthvttpqjc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yonumen.top/gtkqrdgjwc.html

[Q74] 强制使用索引
来源：http://hz.dashuyun.cn/gtmegjvgfd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.meibo888.top/gtqbssezxt.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gtdgfjdqfp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhengqikj.top/gtelyhtrew.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangkeji.top/gtipefxaer.html

[Q76] 按天统计
来源：http://hz.fzhhl.top/gtfqlpjakx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.andypj.xyz/gttemmxwua.html

[Q77] 时间加减
来源：http://hz.yj202588.top/gtceckmyui.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.feifeiyinyue.top/gtjliwuqov.html

[Q78] 当前时间
来源：http://hz.yueranfly.top/gtiwssgnvw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shangyingyoupin.top/gtbddrlvab.html

[Q79] 字符串拼接
来源：http://hz.mhx1999.top/gtldfnzzuk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.smart0.xyz/gtjpopgqly.html

[Q80] 字符串截取
来源：http://hz.havefunace.top/gtgqejcrvy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xinyue.icu/gtrkwpfavt.html

[Q81] 字符串替换
来源：http://hz.hnqzz.top/gtpybfxxlo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.pycfn.com/gtfwdjpzfn.html

[Q82] 字符长度与字节长度
来源：http://hz.yuxming.cn/gtzubkmusy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xziqi.cn/gtyoplhakr.html

[Q83] 大小写转换
来源：http://hz.yj20258.top/gtqtivoweq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.bjfxy.top/gtgxtpwbju.html

[Q84] 去除首尾空格
来源：http://hz.hysaishi.cn/gtjmuzratx.html

SELECT TRIM(name) FROM users;
来源：http://hz.smart0.xyz/gtveesdkhh.html

[Q85] 数值取整
来源：http://hz.yuxming.cn/gtevegpgjn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ivvv.top/gttlpqhyoo.html

[Q86] 读取 JSON 字段
来源：http://hz.sufxvd.cn/gtmypajats.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jlsjyb.cn/gtswopbumc.html

[Q87] JSON 字段做条件
来源：http://hz.ydzc1.top/gtjthuwznp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shuidangran.top/gtkoiifqsh.html

[Q88] 行转列（条件聚合）
来源：http://hz.cucudq.cn/gtdokortfz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nwbrower.top/gtgfdpmego.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jiagoushi.top/gtpokbrczj.html

[Q89] 判断表是否存在
来源：http://hz.feifeiyinyue.top/gtbrdogxpb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.smart0.xyz/gtgjazwzpz.html

[Q90] 生成序号列
来源：http://hz.jinyuanbaomall.cn/gtibnpebcg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hongshengwenyu.top/gtggxrkzsz.html

================================================================================
来源：http://hz.zhengqikj.top/gtlrzwpcen.html

R. Bash 专题
来源：http://hz.yuxming.cn/gtkgokulrf.html

================================================================================
来源：http://hz.tianlin.xyz/gtrtvxtlhm.html

[R01] shebang 与严格模式
来源：http://hz.cdnleiting.top/gtpmiuypxt.html

#!/usr/bin/env bash
来源：http://hz.0kj1m.cn/gtqmxrkctj.html

set -euo pipefail
来源：http://hz.shanyushiyangtech.top/gtbmrajpnm.html

[R02] 变量赋值与使用
来源：http://hz.aibaodan.cn/gtvkcejvju.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangtech.top/gtfpvedxzo.html

[R03] 只读变量
来源：http://hz.ywan-chungtsiang.top/gtoetescvv.html

readonly PI=3.14
来源：http://hz.svipenyu.cn/gtzdwxinhv.html

[R04] 位置参数
来源：http://hz.sweek.top/gtgwdtfppc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yonumen.top/gtmsmewyxg.html

[R05] 参数默认值
来源：http://hz.jinqigufen.top/gtalrbkcpz.html

name="${1:-default}"
来源：http://hz.yj20258888.top/gtpizncekf.html

[R06] 判断命令是否存在
来源：http://hz.zhengqikj.top/gttacujcrg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.meibo888.top/gtjcmonsol.html

[R07] if 判断文件
来源：http://hz.havefunace.top/gtadcurfrj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gaohongyu789.top/gtiklpedjz.html

[R08] 数值比较
来源：http://hz.yj20258888.top/gtmiktspwn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shuidangran.top/gtrqrdubjm.html

[R09] 字符串比较
来源：http://hz.xinyue.icu/gtlzlkjwbj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.nanxinkj.top/gtucpleyqq.html

[R10] 正则匹配
来源：http://hz.svipenyu.cn/gtcnordsdu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.mhx1999.top/gtacmcvlqx.html

[R11] case 多分支
来源：http://hz.chenzaomai.com/gtovdoztgq.html

case "$1" in
来源：http://hz.tian-w.cn/gtdgrvcybr.html

start) echo "启动" ;;
来源：http://hz.iojbl.cn/gtbauwcddu.html

stop)  echo "停止" ;;
来源：http://hz.xziqi.cn/gtbhnsdshu.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtnjzekepy.html

esac
来源：http://hz.0kj1m.cn/gtneyepofb.html

[R12] for 遍历文件
来源：http://hz.9152youxi.cn/gtyymyykkp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuxming.cn/gtyworkazk.html

[R13] for 计数循环
来源：http://hz.aibaodan.cn/gtjxgodmta.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtkvlrnbhr.html

[R14] C 风格 for
来源：http://hz.wangdashe.top/gtrbwejrcb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtlopskzmw.html

[R15] while 逐行读文件
来源：http://hz.jinqigfzy.top/gtiagnztft.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.9152youxi.cn/gtgciqnjoj.html

[R16] until 等待条件
来源：http://hz.nanxinkj.top/gtbfirkvlh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tanke756.top/gtzwldbktf.html

[R17] 数组定义与取值
来源：http://hz.gzhubu.top/gtcmlamfdg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gtwwqyjyhw.html

[R18] 遍历数组
来源：http://hz.shanyushiyangkeji.top/gtpewvymfx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shangyingyoupin.top/gtlgnotyxo.html

[R19] 数组长度
来源：http://hz.nanxinkj.top/gtsiuokrpq.html

echo "${#arr[@]}"
来源：http://hz.chenzaomai.com/gtdoxkjjfe.html

[R20] 关联数组（字典）
来源：http://hz.xziqi.cn/gtrlbfznio.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nwbrower.top/gtqltxexij.html

[R21] 字符串长度
来源：http://hz.yanxiufei.cn/gtswxfrdrj.html

echo "${#s}"
来源：http://hz.shanyushiyangtech.top/gtopwmmmam.html

[R22] 截取子串
来源：http://hz.yanxiufei.cn/gtfoefvppk.html

echo "${s:0:5}"
来源：http://hz.9152youxi.cn/gttpnqyajz.html

[R23] 字符串替换
来源：http://hz.zhixingplan.top/gtiimuuayn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gzhubu.top/gtxqaszble.html

[R24] 大小写转换
来源：http://hz.nanxinkj.top/gtkolawktm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenjidiqi.icu/gtyzswadvf.html

[R25] 去后缀 / 去前缀
来源：http://hz.316326.xyz/gtcljuighu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtachkmzoo.html

[R26] 命令替换
来源：http://hz.zhengqikj.top/gtmwtszgyz.html

now=$(date +%F); echo "$now"
来源：http://hz.316326.xyz/gtfxjngzvk.html

[R27] 算术展开
来源：http://hz.nwbrower.top/gtmxpovxfb.html

echo $((1 + 2 * 3))
来源：http://hz.havefunace.top/gtzfnsertn.html

[R28] 浮点运算
来源：http://hz.ppjwa.cn/gtcmwmyrih.html

echo "scale=2; 10/3" | bc
来源：http://hz.xylfe.cn/gtisdahgst.html

[R29] 定义函数
来源：http://hz.smart0.xyz/gtxmmmvoee.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinqigufen.top/gtsrkwukhk.html

[R30] 函数返回状态码
来源：http://hz.jyoumei.cn/gtacepximh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aizwys.cn/gtnfrkhmjf.html

[R31] 局部变量
来源：http://hz.hnqzz.top/gtrvvpzepy.html

f() { local x=1; echo "$x"; }
来源：http://hz.shzxlz.cn/gtilsmbzyw.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangtech.top/gtkrwciznj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.svipenyu.cn/gtdncxsbri.html

[R33] 捕获错误并提示行号
来源：http://hz.yanxiufei.cn/gtvhsbkloj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhijiandao.cn/gtqgvcnffc.html

[R34] 退出时清理
来源：http://hz.wangdashe.top/gtcxvvwhha.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sufxvd.cn/gtezfajtis.html

[R35] 后台执行并等待
来源：http://hz.zycfv.cn/gtwhxumgjv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ybcxt.top/gtyaxyyocs.html

[R36] 并发执行多个任务
来源：http://hz.andypj.xyz/gtgiiqcpep.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sysykeji.top/gtlylswclx.html

[R37] 把输出赋给变量
来源：http://hz.gaohongyu789.top/gttwgtycqn.html

files=$(ls -1)
来源：http://hz.chenlongwang.top/gtyxwyhetp.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtvsfekcgw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shuidangran.top/gtfxzcwsyl.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtqvggzviz.html

cmd > out.log 2>&1
来源：http://hz.sweek.top/gtsnzpsefb.html

[R40] 追加写日志
来源：http://hz.hywenlv.cn/gtnytqufgp.html

echo "log" >> out.log
来源：http://hz.shanyushiyangkeji.top/gttqfpvlzx.html

[R41] 丢弃输出
来源：http://hz.sweek.top/gtbbuhukdx.html

cmd >/dev/null 2>&1
来源：http://hz.shuidangran.top/gtdsfsacxm.html

[R42] 输入重定向
来源：http://hz.iojbl.cn/gtfntpjqcu.html

wc -l < a.txt
来源：http://hz.cucudq.cn/gtvkehwkqi.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gtvbmrpwud.html

find . -name "*.log" -type f
来源：http://hz.yangfankeji.com/gtswopjdeg.html

[R44] 按修改时间查找
来源：http://hz.yangfankeji.com/gtyfeirsrt.html

find . -mtime -7 -type f
来源：http://hz.snrcjt.cn/gtmfyeovkq.html

[R45] 批量删除
来源：http://hz.zhongyouzk.top/gtojamoszw.html

find . -name "*.tmp" -delete
来源：http://hz.pengpengdd.cyou/gtksehmnyn.html

[R46] 递归替换文件内容
来源：http://hz.yongpay.top/gtiqfnfsir.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cashguo.top/gtpnyiqsdr.html

[R47] sed 单行替换
来源：http://hz.wangdashe.top/gtyufpvffc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.0kj1m.cn/gtvkthczbc.html

[R48] awk 取指定列
来源：http://hz.shuidangran.top/gtmyaagpyw.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhixingplan.top/gtfimagxmq.html

[R49] awk 带条件
来源：http://hz.shangyingyoupin.top/gtuzvvqwtw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yonumen.top/gtcpzxrflm.html

[R50] awk 求和
来源：http://hz.zhaomingkeji.xyz/gtcxgzydbi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gaohongyu789.top/gtnecuuvhq.html

[R51] 排序去重取前几
来源：http://hz.tian-w.cn/gtyfoecfqa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cashguo.top/gtifzkbvfh.html

[R52] 统计行数
来源：http://hz.gotoacloud.top/gtnfqqdlma.html

wc -l a.txt
来源：http://hz.daria6918.cn/gtoasrmofd.html

[R53] 查看文件头与实时尾
来源：http://hz.chenjidiqi.icu/gtytwfjdas.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhengqikj.top/gtzginqmbz.html

[R54] 比较两个文件
来源：http://hz.gogol.net.cn/gttoyqlwtp.html

diff a.txt b.txt
来源：http://hz.yongpay.top/gtvbsbtlpx.html

[R55] 压缩与解压
来源：http://hz.yuxming.cn/gttwgdhxcp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenjidiqi.icu/gttexbnakz.html

[R56] 远程拷贝
来源：http://hz.sysykeji.top/gttpypdapb.html

scp file user@host:/path/
来源：http://hz.zhaomingkeji.xyz/gtunngabyu.html

[R57] 远程执行命令
来源：http://hz.jqgfzy.top/gtgebrqllk.html

ssh user@host 'uptime'
来源：http://hz.sweek.top/gtbctwdagr.html

[R58] 下载文件
来源：http://hz.andypj.xyz/gtvmhjlcmd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.dashuyun.cn/gtfnocgumz.html

[R59] 发 POST JSON
来源：http://hz.yonumen.top/gtaxgxtqvw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.52xcode.cn/gtnoevxnpc.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gtgspchkgr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.aibaodan.cn/gtlwhmqwqx.html

[R61] 磁盘占用
来源：http://hz.havefunace.top/gtyrydlcaf.html

df -h;  du -sh *
来源：http://hz.ywan-chungtsiang.top/gtzcyaievn.html

[R62] 找最占空间的文件
来源：http://hz.yonumen.top/gtoddepobi.html

du -ah . | sort -rh | head -10
来源：http://hz.guowangkeji.top/gtjjielkfi.html

[R63] 内存与进程
来源：http://hz.jqgfzy.top/gtgnaealgr.html

free -h;  ps aux | grep nginx
来源：http://hz.cdnleiting.top/gtgpmmuker.html

[R64] 结束进程
来源：http://hz.sweek.top/gtdljjfhsp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhengqikj.top/gtndjorabo.html

[R65] 查看端口占用
来源：http://hz.c1oappe.top/gtmllhcrok.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.quarkkingdee.top/gtfhrbffwf.html

[R66] 定时任务
来源：http://hz.aizwys.cn/gtoxgsxmkh.html

crontab -e;  crontab -l
来源：http://hz.chenjidiqi.icu/gtxtaluvop.html

[R67] 生成随机十六进制串
来源：http://hz.fzhhl.top/gtsabxlmsu.html

openssl rand -hex 16
来源：http://hz.xingfuxueyuan.xyz/gtgmipkeip.html

[R68] 计算文件校验值
来源：http://hz.yuxming.cn/gtozwcskhk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sweek.top/gtpxlhlvpo.html

[R69] 生成随机密码
来源：http://hz.wangdashe.top/gtwuskmcyz.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinyuanbaomall.cn/gtdcijnuld.html

[R70] 时间戳与互转
来源：http://hz.yj202588.top/gtlrftjqfk.html

date +%s;  date -d @1700000000
来源：http://hz.sysykeji.top/gtwbtlewnp.html

[R71] 日期格式化
来源：http://hz.52xcode.cn/gtluidsdxp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ehwqpu.com/gtoszkvjru.html

[R72] 等待端口就绪
来源：http://hz.316326.xyz/gtyzggklhk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtdhrwxuqb.html

[R73] 分割大日志
来源：http://hz.bjfxy.top/gtqubgvici.html

split -l 1000 big.log part_
来源：http://hz.nanxuanxn.top/gtvmvhzste.html

[R74] 批量重命名
来源：http://hz.shzxlz.cn/gtqbkgrfqd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hongshengwenyu.top/gtadyusuyk.html

[R75] 导出环境变量
来源：http://hz.zhongyouzk.top/gtqzpqyxws.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tanke756.top/gtirgryaxa.html

[R76] 使用临时文件
来源：http://hz.svipenyu.cn/gtqlurlfcs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtmyddvbxl.html

[R77] 读取用户输入
来源：http://hz.52xcode.cn/gtzgfefyot.html

read -rp "请输入: " ans
来源：http://hz.ppjwa.cn/gtshunalti.html

[R78] 交互式菜单
来源：http://hz.ppjwa.cn/gtzgfsrobk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xuanzx.com/gtebjwkicv.html

[R79] 解析命令行选项
来源：http://hz.52xcode.cn/gtfrmzywko.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xuanzx.com/gtlquhgjfl.html

[R80] 查看脚本执行耗时
来源：http://hz.yonumen.top/gthwjslmdi.html

time ./run.sh
来源：http://hz.yongpay.top/gtpekmjrlx.html

================================================================================
来源：http://hz.hfpthk.cn/gtekoiuycn.html

S. C / C++ 专题
来源：http://hz.xziqi.cn/gtkhvyoapz.html

================================================================================
来源：http://hz.havefunace.top/gthghpibeu.html

[S01] C：Hello World
来源：http://hz.yj20258.top/gthjjyumym.html

#include <stdio.h>
来源：http://hz.xingfuxueyuan.xyz/gttyygwbjl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.guowangkeji.top/gtitwdbclw.html

[S02] C：变量与格式化输出
来源：http://hz.smart0.xyz/gtzcadcnsp.html

int a = 10; printf("%d\n", a);
来源：http://hz.gogol.net.cn/gtbfuxywps.html

[S03] C：读入整数
来源：http://hz.shanyushiyangtech.top/gtilxjplfl.html

int x; scanf("%d", &x);
来源：http://hz.dashuyun.cn/gtnltfeesn.html

[S04] C：字符串复制
来源：http://hz.zhongyouzk.top/gtqplwygip.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xuanzx.com/gtwornqypj.html

[S05] C：字符串长度
来源：http://hz.wangdashe.top/gtinggxwfl.html

strlen(s)
来源：http://hz.zhengqikj.top/gtckoiphrv.html

[S06] C：字符串比较
来源：http://hz.shangyingyoupin.top/gtejwpsasb.html

strcmp(a, b) == 0
来源：http://hz.ivvv.top/gtqqdqpqoc.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtsfauwubd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.vqdsnc.cn/gthftihkoh.html

[S08] C：动态内存分配与释放
来源：http://hz.svipenyu.cn/gtqbhjfgxq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.quarkkingdee.top/gtrypmrsbs.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgfzy.top/gtbxqgghcz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zdqjudy.top/gthlmgxpkz.html

[S10] C：指针与解引用
来源：http://hz.yvedp.cn/gtiqgqstsb.html

int *p = &a;  *p = 5;
来源：http://hz.pycfn.com/gtwgkspuux.html

[S11] C：逐行读文件
来源：http://hz.zhixingplan.top/gtrbmvlbgt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hysaishi.cn/gtjtggmezj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cucudq.cn/gtkhdrfvsg.html

fclose(f);
来源：http://hz.mhx1999.top/gtgffwaqjp.html

[S12] C：写文件
来源：http://hz.xingfuxueyuan.xyz/gtbupgvvqm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.316326.xyz/gtytolidsn.html

[S13] C：宏定义
来源：http://hz.shanyushiyangkeji.top/gtwgszxpgd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.feifeiyinyue.top/gtflbcfzri.html

[S14] C：枚举
来源：http://hz.jqgufenzy.top/gtbnpevqfz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fzhhl.top/gtixsaidzp.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtnnmpwisy.html

(double) a / b
来源：http://hz.zhongyouzk.top/gtmnbtaawc.html

[S16] C：位操作置位
来源：http://hz.quarkkingdee.top/gtwbqxkixm.html

x |= (1 << 3);
来源：http://hz.zhengqikj.top/gtcnbsqbfx.html

[S17] C：安全拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtrwmvroix.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.fzhhl.top/gtidvrodiv.html

[S18] C：命令行参数
来源：http://hz.tian-w.cn/gtmkqguobi.html

int main(int argc, char **argv)
来源：http://hz.sxryk.cn/gtwktwkbuw.html

[S19] C：快速排序
来源：http://hz.sweek.top/gtlwrrduib.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gtvqvkvqsz.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtpocycxhh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnqzz.top/gtonfcnbvc.html

[S21] C：字符类别判断
来源：http://hz.zhiwuduotai.top/gtfgoiprsg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xylfe.cn/gtwvkgtcwj.html

[S22] C：字符串转数字
来源：http://hz.yuanzhike.top/gtmentcdiu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.svipenyu.cn/gttastpzrx.html

[S23] C：随机数
来源：http://hz.feifeiyinyue.top/gtxsimeyuz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gaohongyu789.top/gtzdqetjje.html

[S24] C：获取本地时间
来源：http://hz.yuanzhike.top/gtvoaydpsq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.andypj.xyz/gtyqksrdsg.html

[S25] C：内存拷贝
来源：http://hz.jqgfzy.top/gtkbgmkvbg.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtzjqwmkjt.html

[S26] C：内存清零
来源：http://hz.sweek.top/gtfmuqtggr.html

memset(a, 0, sizeof a);
来源：http://hz.snrcjt.cn/gtitubakel.html

[S27] C：定义常量
来源：http://hz.jinyuanbaomall.cn/gtnwacqjdr.html

const double PI = 3.14159;
来源：http://hz.ydzc1.top/gtldldqfau.html

[S28] C：静态变量
来源：http://hz.zhijiandao.cn/gtosrkyfxh.html


<!-- 参考信息 -->