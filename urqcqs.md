代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnxiangtu.top/gtcvcauxwh.html

[Q60] 取上一行 / 下一行
来源：http://hz.meibo888.top/gtprtddrog.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.9152youxi.cn/gtdpauizqo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.52xcode.cn/gtnptqfkzb.html

[Q61] 移动平均
来源：http://hz.shangyingyoupin.top/gtwagmztce.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zdqjudy.top/gtoaigiwcn.html

[Q62] 分组占比
来源：http://hz.xinyue.icu/gtmqxcwyoe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtzamkfkpe.html

[Q63] 开启事务
来源：http://hz.shangyingyoupin.top/gthfyeltff.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.316326.xyz/gtcxdnsxgz.html

[Q64] 提交事务
来源：http://hz.sysykeji.top/gtmxkkmwax.html

COMMIT;
来源：http://hz.ybcxt.top/gttngrsgub.html

[Q65] 回滚事务
来源：http://hz.tianlin.xyz/gtlqrnbrdm.html

ROLLBACK;
来源：http://hz.shzxlz.cn/gteghdmzcd.html

[Q66] 行锁查询
来源：http://hz.svipenyu.cn/gtjrypgkda.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.52xcode.cn/gtbofqgsyf.html

[Q67] 设置隔离级别
来源：http://hz.havefunace.top/gtxiywuxgb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hongshengwenyu.top/gtivlzqsdj.html

[Q68] 保存点
来源：http://hz.shzxlz.cn/gtpzpidbcw.html

SAVEPOINT sp1;
来源：http://hz.wangdashe.top/gtkchzlcya.html

ROLLBACK TO sp1;
来源：http://hz.feifeiyinyue.top/gtxlpkvgij.html

[Q69] 查看执行计划
来源：http://hz.redwolf501.top/gtjqcjqmof.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenzaomai.com/gtwcojqmpg.html

[Q70] 更新统计信息
来源：http://hz.yueranfly.top/gtjouumuey.html

ANALYZE TABLE users;
来源：http://hz.shzxlz.cn/gtqaytksrd.html

[Q71] 查看建表语句
来源：http://hz.zycfv.cn/gtohffvdub.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangshuangyany.cn/gtfsmlmfcj.html

[Q72] 查看索引
来源：http://hz.ydjk.org.cn/gtkoeocpuz.html

SHOW INDEX FROM users;
来源：http://hz.nanxuanxn.top/gtxgazpqks.html

[Q73] 查看表状态
来源：http://hz.jyoumei.cn/gtwtxknqda.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxuanxn.top/gtiftkzjvr.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gtrywwlldj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxuanxn.top/gtqqujuyfi.html

[Q75] 日期格式化
来源：http://hz.ybcxt.top/gtldynkzpt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yongpay.top/gtfmiiphtc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.birdmap.top/gtlgedcivk.html

[Q76] 按天统计
来源：http://hz.jqgufenzy.top/gtdabplwzy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yvedp.cn/gtbdpkujns.html

[Q77] 时间加减
来源：http://hz.hammf.cn/gtgehnpelp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tanke756.top/gtgyffdldj.html

[Q78] 当前时间
来源：http://hz.yj20258888.top/gtqzrluxmk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cheryme.top/gtfrxcpwbn.html

[Q79] 字符串拼接
来源：http://hz.nanxinkj.top/gtttatfzjh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnxiangtu.top/gtanfjmdfc.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gtsjlqnuww.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.mhx1999.top/gtxgxsasgg.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gtwrqrdefk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.316326.xyz/gthpnnwpez.html

[Q82] 字符长度与字节长度
来源：http://hz.quarkkingdee.top/gtucsmxver.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zdqjudy.top/gtciiuttgp.html

[Q83] 大小写转换
来源：http://hz.cucudq.cn/gtaamgspow.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yanxiufei.cn/gtiqayvqxg.html

[Q84] 去除首尾空格
来源：http://hz.316326.xyz/gtvakrvnzq.html

SELECT TRIM(name) FROM users;
来源：http://hz.ivvv.top/gtqnqmppvi.html

[Q85] 数值取整
来源：http://hz.meibo888.top/gtfcuzwnul.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhixingplan.top/gtpbafrgui.html

[Q86] 读取 JSON 字段
来源：http://hz.hammf.cn/gtcfmazuyr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258.top/gtmsfgcppn.html

[Q87] JSON 字段做条件
来源：http://hz.cashguo.top/gttgenkhdt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tanke756.top/gtfehtxqyx.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnqzz.top/gtnqmjonkv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.aibaodan.cn/gtkaxmbaak.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhixingplan.top/gthnlheprl.html

[Q89] 判断表是否存在
来源：http://hz.jinqigfzy.top/gthxcshrxc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ehwqpu.com/gtuggizsvr.html

[Q90] 生成序号列
来源：http://hz.316326.xyz/gtaobsfsdv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yvedp.cn/gtysvzgzto.html

================================================================================
来源：http://hz.yj20258888.top/gtakhpgxdw.html

R. Bash 专题
来源：http://hz.bjfxy.top/gtkqpyvqch.html

================================================================================
来源：http://hz.bjfxy.top/gtrtyscfwx.html

[R01] shebang 与严格模式
来源：http://hz.haohaochexian.top/gtxfvgxlfn.html

#!/usr/bin/env bash
来源：http://hz.hnxiangtu.top/gtiurjpqog.html

set -euo pipefail
来源：http://hz.guannengcc.top/gtkqnrepqf.html

[R02] 变量赋值与使用
来源：http://hz.xziqi.cn/gtnbxuxcxu.html

name="Tom"; echo "$name"
来源：http://hz.yuxming.cn/gtjhswqnuw.html

[R03] 只读变量
来源：http://hz.yuanzhike.top/gtxlrilyrn.html

readonly PI=3.14
来源：http://hz.shzxlz.cn/gtvuezwxyl.html

[R04] 位置参数
来源：http://hz.daria6918.cn/gtqovdjmnv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtzylycpni.html

[R05] 参数默认值
来源：http://hz.yongpay.top/gttgnzpcaw.html

name="${1:-default}"
来源：http://hz.jqgufenzy.top/gtebazdnfi.html

[R06] 判断命令是否存在
来源：http://hz.316326.xyz/gtauanaysm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gttvvvffvn.html

[R07] if 判断文件
来源：http://hz.cqqwz.cn/gtfjkiwzom.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangdashe.top/gtfjydebwt.html

[R08] 数值比较
来源：http://hz.shanyushiyangtech.top/gtlooasile.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinghuilouyu.cn/gtkybdhejn.html

[R09] 字符串比较
来源：http://hz.chenzaomai.com/gtpgcwuwmp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.iojbl.cn/gtwigmwzwn.html

[R10] 正则匹配
来源：http://hz.zhoulong.xyz/gttywsuaey.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuxming.cn/gtxmmlpwlc.html

[R11] case 多分支
来源：http://hz.sysykeji.top/gtbpfjndxa.html

case "$1" in
来源：http://hz.ydjk.org.cn/gtyiwjcwtz.html

start) echo "启动" ;;
来源：http://hz.jinyuanbaomall.cn/gtutwugtem.html

stop)  echo "停止" ;;
来源：http://hz.zhoulong.xyz/gtxnshgdqj.html

*)     echo "未知命令" ;;
来源：http://hz.dianchejie.cn/gtkaftxjax.html

esac
来源：http://hz.jinqigfzy.top/gtohjjplmn.html

[R12] for 遍历文件
来源：http://hz.0kj1m.cn/gtyaxjcnni.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinyuanbaomall.cn/gtxfuvsybe.html

[R13] for 计数循环
来源：http://hz.shangyingyoupin.top/gtfcbnqkfc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.snrcjt.cn/gtqtmtwidd.html

[R14] C 风格 for
来源：http://hz.ppjwa.cn/gtdfrgwgti.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gogol.net.cn/gtlqpmgzen.html

[R15] while 逐行读文件
来源：http://hz.zhiwuduotai.top/gtuexcijxa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dashuyun.cn/gtoteppoww.html

[R16] until 等待条件
来源：http://hz.yonumen.top/gtkozbpqiu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtjivzikmg.html

[R17] 数组定义与取值
来源：http://hz.shuidangran.top/gtuyjezerc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xylfe.cn/gteffklmso.html

[R18] 遍历数组
来源：http://hz.zhijiandao.cn/gtjwltzqcc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhiwuduotai.top/gtvccntysm.html

[R19] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtmhewtgwy.html

echo "${#arr[@]}"
来源：http://hz.snrcjt.cn/gthktoqpuh.html

[R20] 关联数组（字典）
来源：http://hz.hongshengwenyu.top/gtrdnotocc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.feifeiyinyue.top/gtidfyizso.html

[R21] 字符串长度
来源：http://hz.nwbrower.top/gtdfiiwrxr.html

echo "${#s}"
来源：http://hz.nanxinkj.top/gtumachatm.html

[R22] 截取子串
来源：http://hz.guannengcc.top/gtowwlzazz.html

echo "${s:0:5}"
来源：http://hz.jqgufenzy.top/gtoamrkvjq.html

[R23] 字符串替换
来源：http://hz.yuxming.cn/gteageeptz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ydjk.org.cn/gtkybqjiiv.html

[R24] 大小写转换
来源：http://hz.aizwys.cn/gtmuifttho.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigufen.top/gtgyessnmr.html

[R25] 去后缀 / 去前缀
来源：http://hz.hfpthk.cn/gtdknwvsjw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.52xcode.cn/gtgxdcrglb.html

[R26] 命令替换
来源：http://hz.shangyingyoupin.top/gtseookzro.html

now=$(date +%F); echo "$now"
来源：http://hz.zhengqikj.top/gttosyhhsa.html

[R27] 算术展开
来源：http://hz.zhijiandao.cn/gtecibgjkm.html

echo $((1 + 2 * 3))
来源：http://hz.haohaochexian.top/gtoutaakvn.html

[R28] 浮点运算
来源：http://hz.jqgufenzy.top/gtguuomkqz.html

echo "scale=2; 10/3" | bc
来源：http://hz.9152youxi.cn/gtzuatuumo.html

[R29] 定义函数
来源：http://hz.sufxvd.cn/gtuiomofpg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sxryk.cn/gtfaeokgjz.html

[R30] 函数返回状态码
来源：http://hz.kuanghao11.cn/gtnezhkprp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.snrcjt.cn/gtvoodlpbd.html

[R31] 局部变量
来源：http://hz.daxiang520.top/gthxmnyiur.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtlygaqcce.html

[R32] 参数个数校验
来源：http://hz.yj202588.top/gtagropitr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuxming.cn/gtfgyojzqs.html

[R33] 捕获错误并提示行号
来源：http://hz.tian-w.cn/gtjjjjmbjy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jlsjyb.cn/gtywtmdssu.html

[R34] 退出时清理
来源：http://hz.xingfuxueyuan.xyz/gtwfibzqoo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtciovjsii.html

[R35] 后台执行并等待
来源：http://hz.tanke756.top/gtheolzfru.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangkeji.top/gthhamujgj.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtmuwdumme.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dashuyun.cn/gtzrogvglq.html

[R37] 把输出赋给变量
来源：http://hz.haohaochexian.top/gtejqfaoaf.html

files=$(ls -1)
来源：http://hz.ydzc1.top/gttwryekgb.html

[R38] 管道串联
来源：http://hz.fengsongda.top/gtouffgamc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuanzhike.top/gtxqavawkr.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangtech.top/gtvijbinbi.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtlrkkwycf.html

[R40] 追加写日志
来源：http://hz.iojbl.cn/gtvxxakzmx.html

echo "log" >> out.log
来源：http://hz.yanxiufei.cn/gtkyjofqri.html

[R41] 丢弃输出
来源：http://hz.yuxming.cn/gtuypoipdm.html

cmd >/dev/null 2>&1
来源：http://hz.ydjk.org.cn/gtdrljqjfp.html

[R42] 输入重定向
来源：http://hz.nanxinkj.top/gtsgqeuyao.html

wc -l < a.txt
来源：http://hz.wangdashe.top/gtafexxumo.html

[R43] 按名字查找文件
来源：http://hz.tanke756.top/gtorvsdxln.html

find . -name "*.log" -type f
来源：http://hz.ybcxt.top/gtztegkwuv.html

[R44] 按修改时间查找
来源：http://hz.hnxiangtu.top/gtlntxdgnt.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangtech.top/gtydqcwrkf.html

[R45] 批量删除
来源：http://hz.iojbl.cn/gttfyyqgie.html

find . -name "*.tmp" -delete
来源：http://hz.cqqwz.cn/gtkdymialm.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtgnkpixci.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.havefunace.top/gtfcctzkee.html

[R47] sed 单行替换
来源：http://hz.nanxuanxn.top/gtidnoothd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yongpay.top/gtilmtrdma.html

[R48] awk 取指定列
来源：http://hz.chenjidiqi.icu/gtdshzhgla.html

awk '{print $1, $3}' a.txt
来源：http://hz.sxryk.cn/gtujpiukpl.html

[R49] awk 带条件
来源：http://hz.pengpengdd.cyou/gtcxearczt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhixingplan.top/gtimkhllsp.html

[R50] awk 求和
来源：http://hz.havefunace.top/gtdjrscxqp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.bjfxy.top/gtupisakre.html

[R51] 排序去重取前几
来源：http://hz.chenjidiqi.icu/gtvwxdzyag.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.316326.xyz/gtjxlppleu.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtfbobsgzl.html

wc -l a.txt
来源：http://hz.jinqigfzy.top/gtxinaigek.html

[R53] 查看文件头与实时尾
来源：http://hz.jinyuanbaomall.cn/gtkmwftqxr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ehwqpu.com/gtxtzppuyr.html

[R54] 比较两个文件
来源：http://hz.xziqi.cn/gttfshmaui.html

diff a.txt b.txt
来源：http://hz.nanxuanxn.top/gtszizfzup.html

[R55] 压缩与解压
来源：http://hz.zycfv.cn/gtlouutnjk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dianchejie.cn/gthzyptluc.html

[R56] 远程拷贝
来源：http://hz.pycfn.com/gtgsuevruu.html

scp file user@host:/path/
来源：http://hz.zhengqikj.top/gthesepmll.html

[R57] 远程执行命令
来源：http://hz.ehwqpu.com/gtdtfvavlf.html

ssh user@host 'uptime'
来源：http://hz.zycfv.cn/gtwbrgjdqh.html

[R58] 下载文件
来源：http://hz.shanyushiyangtech.top/gtujnyigpm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hammf.cn/gtdvojxzeq.html

[R59] 发 POST JSON
来源：http://hz.guannengcc.top/gtrkazcwez.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gogol.net.cn/gtnxibokhx.html

[R60] 只看 HTTP 状态码
来源：http://hz.tanke756.top/gttscprvep.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daxiang520.top/gtkjblhhyv.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gtrbnlxgxm.html

df -h;  du -sh *
来源：http://hz.zhongyouzk.top/gtekyccxin.html

[R62] 找最占空间的文件
来源：http://hz.ywan-chungtsiang.top/gtzwobrasr.html

du -ah . | sort -rh | head -10
来源：http://hz.pengpengdd.cyou/gtqnjnpjdi.html

[R63] 内存与进程
来源：http://hz.hfpthk.cn/gttljutwkc.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgufenzy.top/gtmqifkfjb.html

[R64] 结束进程
来源：http://hz.fzhhl.top/gtgjkufcdy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guowangkeji.top/gtyjwlpukm.html

[R65] 查看端口占用
来源：http://hz.hammf.cn/gtxsjfysrb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhixingplan.top/gtxjszizsl.html

[R66] 定时任务
来源：http://hz.yvedp.cn/gtenmvzrkr.html

crontab -e;  crontab -l
来源：http://hz.mhx1999.top/gtuoehklax.html

[R67] 生成随机十六进制串
来源：http://hz.ywan-chungtsiang.top/gtmfverawh.html

openssl rand -hex 16
来源：http://hz.iojbl.cn/gtcwszxtxx.html

[R68] 计算文件校验值
来源：http://hz.zdqjudy.top/gttsdckxan.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yuxming.cn/gtardnykqr.html

[R69] 生成随机密码
来源：http://hz.ivvv.top/gtoestcqfg.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangtech.top/gtgdbhckro.html

[R70] 时间戳与互转
来源：http://hz.jyoumei.cn/gtlxjpbuij.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtwovbervw.html

[R71] 日期格式化
来源：http://hz.gaohongyu789.top/gtldwfclgt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.redwolf501.top/gtljuelxii.html

[R72] 等待端口就绪
来源：http://hz.yuxming.cn/gtemyaaocn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.snrcjt.cn/gtvzxnaqik.html

[R73] 分割大日志
来源：http://hz.ywan-chungtsiang.top/gtxoguxpkf.html

split -l 1000 big.log part_
来源：http://hz.wangdashe.top/gtrsmzyamy.html

[R74] 批量重命名
来源：http://hz.sweek.top/gtdaghhtwf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.havefunace.top/gtdswkuerg.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtgmjzessh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jyoumei.cn/gtamaaobqc.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtcmpsanuy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuetiantiany.cn/gtwfmwgmjk.html

[R77] 读取用户输入
来源：http://hz.zycfv.cn/gtrugjvami.html

read -rp "请输入: " ans
来源：http://hz.snrcjt.cn/gthgmafdos.html

[R78] 交互式菜单
来源：http://hz.yj20258.top/gtdhneiasv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj202588.top/gtpjzytiqd.html

[R79] 解析命令行选项
来源：http://hz.ppjwa.cn/gtwmltieaw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cdnleiting.top/gtabqzgvua.html

[R80] 查看脚本执行耗时
来源：http://hz.yueranfly.top/gtvjvyfhtj.html

time ./run.sh
来源：http://hz.yj20258888.top/gtpebraigx.html

================================================================================
来源：http://hz.hammf.cn/gteovwhvzk.html

S. C / C++ 专题
来源：http://hz.fzhhl.top/gtpivgsczo.html

================================================================================
来源：http://hz.iojbl.cn/gtsopshkzx.html

[S01] C：Hello World
来源：http://hz.zdqjudy.top/gtjqztzgvh.html

#include <stdio.h>
来源：http://hz.yvedp.cn/gtmbkggjwu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gogol.net.cn/gtnbpfweza.html

[S02] C：变量与格式化输出
来源：http://hz.nwbrower.top/gtfumxmwhj.html

int a = 10; printf("%d\n", a);
来源：http://hz.shangyingyoupin.top/gtgfnmelig.html

[S03] C：读入整数
来源：http://hz.yonumen.top/gtyrepqzdj.html

int x; scanf("%d", &x);
来源：http://hz.hysaishi.cn/gtdyioutav.html

[S04] C：字符串复制
来源：http://hz.nanxinkj.top/gtqkpdrpxe.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydjk.org.cn/gtrlpytrab.html

[S05] C：字符串长度
来源：http://hz.yj202588.top/gtemypcxbc.html

strlen(s)
来源：http://hz.jinqigufen.top/gtcjwvdajf.html

[S06] C：字符串比较
来源：http://hz.zhengqikj.top/gtizvrrfht.html

strcmp(a, b) == 0
来源：http://hz.gaohongyu789.top/gtbjcslwdk.html

[S07] C：数组遍历求和
来源：http://hz.yj202588.top/gtixkcrrtt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigfzy.top/gtelxeaqpx.html

[S08] C：动态内存分配与释放
来源：http://hz.zhijiandao.cn/gtxvdnuzni.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhengqikj.top/gttixhscby.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gteddqeoyf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hammf.cn/gtdfanaztb.html

[S10] C：指针与解引用
来源：http://hz.zhixingplan.top/gtccpbgjbc.html

int *p = &a;  *p = 5;
来源：http://hz.yuxming.cn/gtzagrjhbs.html

[S11] C：逐行读文件
来源：http://hz.gaohongyu789.top/gtjuedkzzh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hnxiangtu.top/gtdcfjdeev.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.kuanghao11.cn/gthxmsyjhd.html

fclose(f);
来源：http://hz.52xcode.cn/gtglgilnen.html

[S12] C：写文件
来源：http://hz.kuanghao11.cn/gtibiojmfg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cheryme.top/gtetkpnvgx.html

[S13] C：宏定义
来源：http://hz.gzhubu.top/gtnkxypwoz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtbecjbdly.html

[S14] C：枚举
来源：http://hz.kuanghao11.cn/gtkjccjchz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhixingplan.top/gtpynsybmm.html

[S15] C：类型转换
来源：http://hz.chenjidiqi.icu/gtchikcnmy.html

(double) a / b
来源：http://hz.gzhubu.top/gtscnxuasd.html

[S16] C：位操作置位
来源：http://hz.xingfuxueyuan.xyz/gtrarkmkzc.html

x |= (1 << 3);
来源：http://hz.kuanghao11.cn/gtbjkxghdn.html

[S17] C：安全拼接字符串
来源：http://hz.tanke756.top/gttmbpzmoa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jyoumei.cn/gtlojdhknd.html

[S18] C：命令行参数
来源：http://hz.jyoumei.cn/gtfhkfqqmf.html

int main(int argc, char **argv)
来源：http://hz.yuanzhike.top/gtwkncvnjm.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gtgvhstinj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gtdkyhdqhv.html

[S20] C：二分查找
来源：http://hz.daxiang520.top/gtnhulyxkd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.birdmap.top/gtpxkwxqgu.html

[S21] C：字符类别判断
来源：http://hz.gaohongyu789.top/gttncqikry.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.52xcode.cn/gtycmpwhxu.html

[S22] C：字符串转数字
来源：http://hz.zhijiandao.cn/gtnwvniesg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gtguuoprzo.html

[S23] C：随机数
来源：http://hz.zhiwuduotai.top/gtmfpweheq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuanzx.com/gtmthmhcox.html

[S24] C：获取本地时间
来源：http://hz.redwolf501.top/gttqkwhluc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shuidangran.top/gtpsswemjh.html

[S25] C：内存拷贝
来源：http://hz.tianlin.xyz/gtmxjunhsc.html

memcpy(dst, src, n);
来源：http://hz.haohaochexian.top/gtelcfsyqc.html

[S26] C：内存清零
来源：http://hz.52xcode.cn/gtcowlpykv.html

memset(a, 0, sizeof a);
来源：http://hz.0kj1m.cn/gtzserrcqc.html

[S27] C：定义常量
来源：http://hz.jinqigufen.top/gttmhvzbel.html

const double PI = 3.14159;
来源：http://hz.meibo888.top/gtuulcuuak.html

[S28] C：静态变量
来源：http://hz.feifeiyinyue.top/gtypvzppsq.html

static int counter = 0;
来源：http://hz.ppjwa.cn/gtefjizsma.html

[S29] C：变参函数
来源：http://hz.zhijiandao.cn/gtuladhdhp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.316326.xyz/gtpugrxeqn.html

[S30] C：头文件保护
来源：http://hz.daria6918.cn/gtbxwadhdi.html


<!-- 参考信息 -->