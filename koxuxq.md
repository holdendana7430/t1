代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ybcxt.top/gtmeuccnmh.html

[Q60] 取上一行 / 下一行
来源：http://hz.jianghu66.top/gtsrhfclvq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jqgfzy.top/gtnputwaym.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yangfankeji.com/gtddfncjvc.html

[Q61] 移动平均
来源：http://hz.fzhhl.top/gtjjbowuph.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tianlin.xyz/gtgrafxtfd.html

[Q62] 分组占比
来源：http://hz.zycfv.cn/gtabxgwafx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.havefunace.top/gticedriee.html

[Q63] 开启事务
来源：http://hz.shuidangran.top/gtinvkbxdi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ivvv.top/gthijaqahd.html

[Q64] 提交事务
来源：http://hz.birdmap.top/gtefuoxwia.html

COMMIT;
来源：http://hz.hnxiangtu.top/gtrsdpiebf.html

[Q65] 回滚事务
来源：http://hz.guannengcc.top/gtghbyeaki.html

ROLLBACK;
来源：http://hz.vqdsnc.cn/gtbktguuad.html

[Q66] 行锁查询
来源：http://hz.zhongyouzk.top/gtcnrdigfh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.mhx1999.top/gtfkkxpcht.html

[Q67] 设置隔离级别
来源：http://hz.tian-w.cn/gtslietovn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jianghu66.top/gtkleygxtg.html

[Q68] 保存点
来源：http://hz.zhixingplan.top/gtahpgpdtx.html

SAVEPOINT sp1;
来源：http://hz.birdmap.top/gtkfiypqoe.html

ROLLBACK TO sp1;
来源：http://hz.chenlongwang.top/gtearrvqkg.html

[Q69] 查看执行计划
来源：http://hz.yuxming.cn/gtwdqkidvf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgfzy.top/gtoifjweoc.html

[Q70] 更新统计信息
来源：http://hz.c1oappe.top/gtboobavug.html

ANALYZE TABLE users;
来源：http://hz.jinqigufen.top/gtpafcamhl.html

[Q71] 查看建表语句
来源：http://hz.ppjwa.cn/gtrbnixsmw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guannengcc.top/gtcktmbsuh.html

[Q72] 查看索引
来源：http://hz.yueranfly.top/gtvbmpoglo.html

SHOW INDEX FROM users;
来源：http://hz.gogol.net.cn/gtkzwlapoh.html

[Q73] 查看表状态
来源：http://hz.yangfankeji.com/gtvvokkkas.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ywan-chungtsiang.top/gtorrszbhw.html

[Q74] 强制使用索引
来源：http://hz.iojbl.cn/gtdhahddbj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.feifeiyinyue.top/gtvpzmlyln.html

[Q75] 日期格式化
来源：http://hz.cucudq.cn/gtqgyitodd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aizwys.cn/gthogwnqqr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.fzhhl.top/gtqjefcxjp.html

[Q76] 按天统计
来源：http://hz.snrcjt.cn/gtmcwhczhq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.aizwys.cn/gtseaziodm.html

[Q77] 时间加减
来源：http://hz.bjfxy.top/gtqbsjours.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtxyousvhr.html

[Q78] 当前时间
来源：http://hz.yonumen.top/gtyynrkzms.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgfzy.top/gtezqawouo.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gthzxrfauz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.316326.xyz/gtkwhpxpjq.html

[Q80] 字符串截取
来源：http://hz.zycfv.cn/gtnicitcti.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dianchejie.cn/gtapyoihor.html

[Q81] 字符串替换
来源：http://hz.jianghu66.top/gtsvnzquii.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.redwolf501.top/gtyvljzfqs.html

[Q82] 字符长度与字节长度
来源：http://hz.smart0.xyz/gtzhqcwtzv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuanzhike.top/gtcmpxxsmc.html

[Q83] 大小写转换
来源：http://hz.shuidangran.top/gtnhlqyjnu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.fzhhl.top/gtcyplvfae.html

[Q84] 去除首尾空格
来源：http://hz.shangyingyoupin.top/gtnvwwmqxs.html

SELECT TRIM(name) FROM users;
来源：http://hz.jqgfzy.top/gtwplcydxs.html

[Q85] 数值取整
来源：http://hz.yj20258.top/gttkudmfyo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.316326.xyz/gturouzbfv.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxuanxn.top/gtptxixdxl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.bjfxy.top/gtvqwpcemn.html

[Q87] JSON 字段做条件
来源：http://hz.smart0.xyz/gtzigynjdf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinghuilouyu.cn/gtcedjegwd.html

[Q88] 行转列（条件聚合）
来源：http://hz.hfpthk.cn/gthkpfofha.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sysykeji.top/gtborpxpjj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zycfv.cn/gtmkblrxjp.html

[Q89] 判断表是否存在
来源：http://hz.52xcode.cn/gtlosueolp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fzhhl.top/gtpcxdpasw.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangtech.top/gtuizleilz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.0kj1m.cn/gtzmvgfjva.html

================================================================================
来源：http://hz.vqdsnc.cn/gtgqvgtrmz.html

R. Bash 专题
来源：http://hz.hywenlv.cn/gtwmqkwbmr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtahwixzvy.html

[R01] shebang 与严格模式
来源：http://hz.cashguo.top/gtalvzgamj.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtdtrfwxvw.html

set -euo pipefail
来源：http://hz.zhoulong.xyz/gtnvvhbwrl.html

[R02] 变量赋值与使用
来源：http://hz.ivvv.top/gtyjahxstg.html

name="Tom"; echo "$name"
来源：http://hz.52xcode.cn/gtjmpqghsw.html

[R03] 只读变量
来源：http://hz.ehwqpu.com/gtpvncsgnv.html

readonly PI=3.14
来源：http://hz.shanyushiyangkeji.top/gtrmwwfumi.html

[R04] 位置参数
来源：http://hz.yuxming.cn/gtejpcyoek.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.daria6918.cn/gtnrneockx.html

[R05] 参数默认值
来源：http://hz.shzxlz.cn/gtfhdiuifg.html

name="${1:-default}"
来源：http://hz.jlsjyb.cn/gtzaottkjb.html

[R06] 判断命令是否存在
来源：http://hz.mhx1999.top/gtlzganzws.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.havefunace.top/gtarrsnzfa.html

[R07] if 判断文件
来源：http://hz.gogol.net.cn/gtbxckaqqg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.9152youxi.cn/gtlrppbbyt.html

[R08] 数值比较
来源：http://hz.bjfxy.top/gtsjuuyemr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ivvv.top/gtjdjkxfik.html

[R09] 字符串比较
来源：http://hz.sweek.top/gtnxuhvqum.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jqgufenzy.top/gtvocxnwow.html

[R10] 正则匹配
来源：http://hz.jinqigufen.top/gtglyecbhb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxuanxn.top/gtdhvivksu.html

[R11] case 多分支
来源：http://hz.ybcxt.top/gtpwjxyemz.html

case "$1" in
来源：http://hz.ehwqpu.com/gtwebikhuv.html

start) echo "启动" ;;
来源：http://hz.yangfankeji.com/gtetulrlsl.html

stop)  echo "停止" ;;
来源：http://hz.nanxinkj.top/gthkhedvak.html

*)     echo "未知命令" ;;
来源：http://hz.zhengqikj.top/gtkwyfifec.html

esac
来源：http://hz.zdqjudy.top/gtjjvveutw.html

[R12] for 遍历文件
来源：http://hz.zhengqikj.top/gtwjnoaolw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yvedp.cn/gthsyoqpmt.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtdakdeazp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtpgjfdoca.html

[R14] C 风格 for
来源：http://hz.pengpengdd.cyou/gtiexedsfw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxuanxn.top/gtkxhpygvd.html

[R15] while 逐行读文件
来源：http://hz.cdnleiting.top/gtftvucbwy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.redwolf501.top/gtvlzokzbc.html

[R16] until 等待条件
来源：http://hz.dashuyun.cn/gtglqsqxgz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guowangkeji.top/gtymsblcsr.html

[R17] 数组定义与取值
来源：http://hz.wangdashe.top/gtbylfjadg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ybcxt.top/gtgxcriwkq.html

[R18] 遍历数组
来源：http://hz.jqgfzy.top/gtlwkkotus.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.9152youxi.cn/gtlnxwucmi.html

[R19] 数组长度
来源：http://hz.birdmap.top/gtraaccddx.html

echo "${#arr[@]}"
来源：http://hz.tian-w.cn/gtycnqebxh.html

[R20] 关联数组（字典）
来源：http://hz.cashguo.top/gtejnpcipu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tanke756.top/gthcjmijyq.html

[R21] 字符串长度
来源：http://hz.jinghuilouyu.cn/gtgodyemow.html

echo "${#s}"
来源：http://hz.aizwys.cn/gtdlnkukrc.html

[R22] 截取子串
来源：http://hz.gzhubu.top/gtzznhgyyh.html

echo "${s:0:5}"
来源：http://hz.52xcode.cn/gtpvdkqvha.html

[R23] 字符串替换
来源：http://hz.jyoumei.cn/gtoelnufhn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhengqikj.top/gtodeclpvi.html

[R24] 大小写转换
来源：http://hz.jianghu66.top/gtzgbqxpiv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhixingplan.top/gtaqumvaqt.html

[R25] 去后缀 / 去前缀
来源：http://hz.ivvv.top/gtegoilbzm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinghuilouyu.cn/gtqoemjmyx.html

[R26] 命令替换
来源：http://hz.jinqigfzy.top/gtzllopxys.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxuanxn.top/gtgrtrjkbu.html

[R27] 算术展开
来源：http://hz.yj20258888.top/gtdargtsen.html

echo $((1 + 2 * 3))
来源：http://hz.cashguo.top/gtcncoycgk.html

[R28] 浮点运算
来源：http://hz.yj20258.top/gtrzhkjztd.html

echo "scale=2; 10/3" | bc
来源：http://hz.cdnleiting.top/gtclwyuvos.html

[R29] 定义函数
来源：http://hz.birdmap.top/gtigixecsd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinqigfzy.top/gtqgwsrzmp.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gtqpvyknvk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nwbrower.top/gtyxyugqod.html

[R31] 局部变量
来源：http://hz.dashuyun.cn/gtgwauxfnq.html

f() { local x=1; echo "$x"; }
来源：http://hz.dashuyun.cn/gtmylxyflx.html

[R32] 参数个数校验
来源：http://hz.zhiwuduotai.top/gtvfpvnqnk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhoulong.xyz/gtshlipouz.html

[R33] 捕获错误并提示行号
来源：http://hz.dianchejie.cn/gtknztjxjf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.fzhhl.top/gtefqvscom.html

[R34] 退出时清理
来源：http://hz.pycfn.com/gtllzehizb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtynemrset.html

[R35] 后台执行并等待
来源：http://hz.sufxvd.cn/gtuixahziv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cucudq.cn/gtbcdcblnw.html

[R36] 并发执行多个任务
来源：http://hz.dashuyun.cn/gtbbktydcz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.bjfxy.top/gtpdecfimv.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gteujrqnle.html

files=$(ls -1)
来源：http://hz.meibo888.top/gtvdqczaoq.html

[R38] 管道串联
来源：http://hz.zhengqikj.top/gtpkwpyxmr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cucudq.cn/gtkikpigod.html

[R39] 重定向标准输出与错误
来源：http://hz.zycfv.cn/gthtwzbocp.html

cmd > out.log 2>&1
来源：http://hz.shangyingyoupin.top/gttjwtwlwb.html

[R40] 追加写日志
来源：http://hz.tanke756.top/gtwtdtihhg.html

echo "log" >> out.log
来源：http://hz.andypj.xyz/gtkuycfrme.html

[R41] 丢弃输出
来源：http://hz.nanxinkj.top/gtpqdodmhh.html

cmd >/dev/null 2>&1
来源：http://hz.zhoulong.xyz/gtbhvbpyiy.html

[R42] 输入重定向
来源：http://hz.cdnleiting.top/gtsnjxzdlo.html

wc -l < a.txt
来源：http://hz.xziqi.cn/gtukmzdkts.html

[R43] 按名字查找文件
来源：http://hz.cdnleiting.top/gtyvmhdlex.html

find . -name "*.log" -type f
来源：http://hz.sweek.top/gtjcjconiv.html

[R44] 按修改时间查找
来源：http://hz.nanxinkj.top/gthlazqbne.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtifkiswty.html

[R45] 批量删除
来源：http://hz.0kj1m.cn/gtgvxzyxit.html

find . -name "*.tmp" -delete
来源：http://hz.sweek.top/gtkymyzuxx.html

[R46] 递归替换文件内容
来源：http://hz.yuxming.cn/gtaitbnqhw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinyuanbaomall.cn/gtleweqkey.html

[R47] sed 单行替换
来源：http://hz.hnqzz.top/gtwwfpkztu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gtgfwjetpf.html

[R48] awk 取指定列
来源：http://hz.yongpay.top/gtqsdzkhxl.html

awk '{print $1, $3}' a.txt
来源：http://hz.shuidangran.top/gtdierngpc.html

[R49] awk 带条件
来源：http://hz.chenzaomai.com/gtadifxcbo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sweek.top/gtkxoxqwta.html

[R50] awk 求和
来源：http://hz.aizwys.cn/gtwhjrdumd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.wangshuangyany.cn/gtugpnujre.html

[R51] 排序去重取前几
来源：http://hz.yuanzhike.top/gtucygipqo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gzhubu.top/gtpphqfjwo.html

[R52] 统计行数
来源：http://hz.jlsjyb.cn/gtipoxghyj.html

wc -l a.txt
来源：http://hz.ivvv.top/gtpyiumepu.html

[R53] 查看文件头与实时尾
来源：http://hz.jiagoushi.top/gtrdduovgy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yueranfly.top/gtbsqqtoje.html

[R54] 比较两个文件
来源：http://hz.gzhubu.top/gtwfucdggg.html

diff a.txt b.txt
来源：http://hz.gzhubu.top/gtmtjebynj.html

[R55] 压缩与解压
来源：http://hz.ydjk.org.cn/gtmoyxurvd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xingfuxueyuan.xyz/gtbsykcpet.html

[R56] 远程拷贝
来源：http://hz.hammf.cn/gtmibyztno.html

scp file user@host:/path/
来源：http://hz.zycfv.cn/gtchgavimh.html

[R57] 远程执行命令
来源：http://hz.zhongyouzk.top/gtwzjiunbn.html

ssh user@host 'uptime'
来源：http://hz.hysaishi.cn/gtmthbunfo.html

[R58] 下载文件
来源：http://hz.svipenyu.cn/gtbwqofwgz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gtqfdqofga.html

[R59] 发 POST JSON
来源：http://hz.bjfxy.top/gtdtsxabgk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jianghu66.top/gtxqcxodns.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gttosdwfpq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinghuilouyu.cn/gtwsnuklcz.html

[R61] 磁盘占用
来源：http://hz.hnxiangtu.top/gtvinyhnjw.html

df -h;  du -sh *
来源：http://hz.shanyushiyangtech.top/gtfswlvwsi.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gtjerjrhum.html

du -ah . | sort -rh | head -10
来源：http://hz.ydjk.org.cn/gtvurcubdy.html

[R63] 内存与进程
来源：http://hz.mhx1999.top/gthdzarhcp.html

free -h;  ps aux | grep nginx
来源：http://hz.hammf.cn/gtpfwomghb.html

[R64] 结束进程
来源：http://hz.gzhubu.top/gtrcpntxaw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nanxinkj.top/gtrtvtchpx.html

[R65] 查看端口占用
来源：http://hz.chenlongwang.top/gtkxgbwrqm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cucudq.cn/gtuxeivgkc.html

[R66] 定时任务
来源：http://hz.hfpthk.cn/gtpruuqgui.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangkeji.top/gtypnrikbt.html

[R67] 生成随机十六进制串
来源：http://hz.c1oappe.top/gtgfpsmtyz.html

openssl rand -hex 16
来源：http://hz.ydzc1.top/gticvzhgos.html

[R68] 计算文件校验值
来源：http://hz.dianchejie.cn/gtkapqddpg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sxryk.cn/gtcxhfyxiu.html

[R69] 生成随机密码
来源：http://hz.yanxiufei.cn/gtwktezxxl.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gtocuectvh.html

[R70] 时间戳与互转
来源：http://hz.sysykeji.top/gtkgpbuxjz.html

date +%s;  date -d @1700000000
来源：http://hz.ybcxt.top/gtgjpvxmrn.html

[R71] 日期格式化
来源：http://hz.pycfn.com/gtfepbzamc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.316326.xyz/gttjtzmict.html

[R72] 等待端口就绪
来源：http://hz.wangdashe.top/gtforftwka.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hnqzz.top/gtcscwftcu.html

[R73] 分割大日志
来源：http://hz.aizwys.cn/gtqqxsazsg.html

split -l 1000 big.log part_
来源：http://hz.gzhubu.top/gtoznmetlh.html

[R74] 批量重命名
来源：http://hz.chenjidiqi.icu/gtswjrkfws.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.c1oappe.top/gtrgbpxbaw.html

[R75] 导出环境变量
来源：http://hz.yvedp.cn/gtrrowpwoc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shuidangran.top/gtnnairyfc.html

[R76] 使用临时文件
来源：http://hz.ppjwa.cn/gtvbtjnoos.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenlongwang.top/gtnaigyfmk.html

[R77] 读取用户输入
来源：http://hz.hfpthk.cn/gtrpokhnfp.html

read -rp "请输入: " ans
来源：http://hz.hfpthk.cn/gtuvciisyv.html

[R78] 交互式菜单
来源：http://hz.yuxming.cn/gtvtcoznrb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hysaishi.cn/gtymdxfblo.html

[R79] 解析命令行选项
来源：http://hz.andypj.xyz/gtyfwelzos.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhongyouzk.top/gtphebhhqh.html

[R80] 查看脚本执行耗时
来源：http://hz.hnqzz.top/gtvoasaruk.html

time ./run.sh
来源：http://hz.feifeiyinyue.top/gtqvtlmumi.html

================================================================================
来源：http://hz.daria6918.cn/gtewzocyqx.html

S. C / C++ 专题
来源：http://hz.shanyushiyangtech.top/gtgxwtwfue.html

================================================================================
来源：http://hz.tian-w.cn/gtvxydyldy.html

[S01] C：Hello World
来源：http://hz.hnxiangtu.top/gtqnyaucit.html

#include <stdio.h>
来源：http://hz.ybcxt.top/gtoksyyfil.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xinyue.icu/gtmrqfrfzo.html

[S02] C：变量与格式化输出
来源：http://hz.jiagoushi.top/gttzgfsasq.html

int a = 10; printf("%d\n", a);
来源：http://hz.tian-w.cn/gtgeivbkzq.html

[S03] C：读入整数
来源：http://hz.gaohongyu789.top/gtglyrguts.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gthnvlkogh.html

[S04] C：字符串复制
来源：http://hz.hongshengwenyu.top/gtwvdmvyeu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cqqwz.cn/gtzpwockkx.html

[S05] C：字符串长度
来源：http://hz.jinqigufen.top/gtqkfbhkqw.html

strlen(s)
来源：http://hz.havefunace.top/gtgtjbaclc.html

[S06] C：字符串比较
来源：http://hz.hammf.cn/gtjczozlcu.html

strcmp(a, b) == 0
来源：http://hz.wangshuangyany.cn/gtoayrgrac.html

[S07] C：数组遍历求和
来源：http://hz.guowangkeji.top/gtiycmmoot.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tian-w.cn/gtdcutmvwo.html

[S08] C：动态内存分配与释放
来源：http://hz.ydjk.org.cn/gtptvchvhd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhaomingkeji.xyz/gtrkgoxxwi.html

[S09] C：结构体定义与初始化
来源：http://hz.andypj.xyz/gtudvshmoi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.316326.xyz/gtenxylsga.html

[S10] C：指针与解引用
来源：http://hz.yongpay.top/gtwatcxgqp.html

int *p = &a;  *p = 5;
来源：http://hz.jyoumei.cn/gtclrhplxq.html

[S11] C：逐行读文件
来源：http://hz.zhixingplan.top/gtqunfwths.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tian-w.cn/gtlfqbnzwn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yongpay.top/gtdjbrhtph.html

fclose(f);
来源：http://hz.xuetiantiany.cn/gtvudszwgv.html

[S12] C：写文件
来源：http://hz.dianchejie.cn/gtqzarqsxn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuetiantiany.cn/gtuvdfxvbg.html

[S13] C：宏定义
来源：http://hz.smart0.xyz/gtpldfxdph.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pengpengdd.cyou/gtbfybpvga.html

[S14] C：枚举
来源：http://hz.zhengqikj.top/gtkmyhnpkd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.feifeiyinyue.top/gttjgivmxm.html

[S15] C：类型转换
来源：http://hz.yangfankeji.com/gtllvmomtp.html

(double) a / b
来源：http://hz.yj20258.top/gtxnejrpcd.html

[S16] C：位操作置位
来源：http://hz.jlsjyb.cn/gtnbuxajkt.html

x |= (1 << 3);
来源：http://hz.ydjk.org.cn/gtjrkyembf.html

[S17] C：安全拼接字符串
来源：http://hz.hnxiangtu.top/gtdqvddvdc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.tian-w.cn/gtphiwovpc.html

[S18] C：命令行参数
来源：http://hz.guannengcc.top/gtnzogqfly.html

int main(int argc, char **argv)
来源：http://hz.ppjwa.cn/gtcrwdvksa.html

[S19] C：快速排序
来源：http://hz.vqdsnc.cn/gtrjocojmu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtpdokvycp.html

[S20] C：二分查找
来源：http://hz.jiagoushi.top/gtjybvqipy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtgjblsetc.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gtipwopspu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.meibo888.top/gtoaqcimzh.html

[S22] C：字符串转数字
来源：http://hz.ehwqpu.com/gtmrmojuzq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.52xcode.cn/gtrptgdazd.html

[S23] C：随机数
来源：http://hz.zhaomingkeji.xyz/gtemcanbia.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pengpengdd.cyou/gtrjvjkaiy.html

[S24] C：获取本地时间
来源：http://hz.cucudq.cn/gtanarfxbs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj202588.top/gtebkatkfa.html

[S25] C：内存拷贝
来源：http://hz.zhijiandao.cn/gtnstzaszr.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtxhxtmztl.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gtnbfbvwdb.html

memset(a, 0, sizeof a);
来源：http://hz.cdnleiting.top/gtwxfyihgy.html

[S27] C：定义常量
来源：http://hz.ppjwa.cn/gthapjduse.html

const double PI = 3.14159;
来源：http://hz.hammf.cn/gtnvgasyas.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gtzxvxjsid.html

static int counter = 0;
来源：http://hz.sxryk.cn/gtdgwbflri.html

[S29] C：变参函数
来源：http://hz.ivvv.top/gtukvuqhal.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.feifeiyinyue.top/gteptjfebe.html

[S30] C：头文件保护
来源：http://hz.0kj1m.cn/gtfuqfkagu.html


<!-- 参考信息 -->