代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangkeji.top/gtgecawgrb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dashuyun.cn/gtqzbdjbwx.html

[Q43] 标量子查询
来源：http://hz.smart0.xyz/gtteeealou.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ybcxt.top/gtneunbris.html

[Q44] IN 子查询
来源：http://hz.hywenlv.cn/gttbsvumls.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aizwys.cn/gtguirwkbk.html

[Q45] EXISTS 判断存在
来源：http://hz.gaohongyu789.top/gtfjjvuhvf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtgyxecejj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinghuilouyu.cn/gtjzlwexsk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tian-w.cn/gtfltkhnci.html

[Q47] 与平均值比较
来源：http://hz.ybcxt.top/gtsmnxhyhg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhijiandao.cn/gtfhrndkid.html

[Q48] CTE 公用表表达式
来源：http://hz.hfpthk.cn/gtxgzpcusp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinyuanbaomall.cn/gtrcoxznfg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydzc1.top/gtcdrsmfvr.html

[Q49] 更新单行
来源：http://hz.haohaochexian.top/gtbkfbxslj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtslpjbtpy.html

[Q50] 批量更新
来源：http://hz.zdqjudy.top/gtlykzgdul.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aibaodan.cn/gtbnymnxrm.html

[Q51] 用子查询更新
来源：http://hz.aizwys.cn/gtmcnjfmuo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinghuilouyu.cn/gtgogfgurd.html

[Q52] 删除指定行
来源：http://hz.ehwqpu.com/gtkmzlbzou.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinyuanbaomall.cn/gtcniiyhgq.html

[Q53] 按条件删除
来源：http://hz.yanxiufei.cn/gtbafnbscb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hywenlv.cn/gtnbcvezne.html

[Q54] 清空表
来源：http://hz.9152youxi.cn/gtnfncturh.html

TRUNCATE TABLE logs;
来源：http://hz.hfpthk.cn/gtstuncxzt.html

[Q55] 排名（并列占位）
来源：http://hz.zhiwuduotai.top/gtjkmyatrv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cashguo.top/gtpilyauer.html

[Q56] 密集排名（并列不占位）
来源：http://hz.vqdsnc.cn/gtieshhaul.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.52xcode.cn/gtivspvaio.html

[Q57] 行号
来源：http://hz.gotoacloud.top/gthqhyzyxs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daxiang520.top/gtojijeuxw.html

[Q58] 累计求和
来源：http://hz.hywenlv.cn/gtqqakylch.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.aibaodan.cn/gtojlcyjmc.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtftythnhh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangtech.top/gthrgvpjsq.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangdashe.top/gtimnidlfs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gotoacloud.top/gtqbzfbolc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenlongwang.top/gtwqgwkahm.html

[Q61] 移动平均
来源：http://hz.feifeiyinyue.top/gtuoavyzes.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hammf.cn/gtzwnjwrxi.html

[Q62] 分组占比
来源：http://hz.ppjwa.cn/gtjybpwgvr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtmfemlgmk.html

[Q63] 开启事务
来源：http://hz.hfpthk.cn/gtajtvmyxk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hysaishi.cn/gtvdrlphae.html

[Q64] 提交事务
来源：http://hz.yanxiufei.cn/gtnwtifdrl.html

COMMIT;
来源：http://hz.yuxming.cn/gtyxczlhty.html

[Q65] 回滚事务
来源：http://hz.xuetiantiany.cn/gtcipfgiwt.html

ROLLBACK;
来源：http://hz.meibo888.top/gtkmpsgtbq.html

[Q66] 行锁查询
来源：http://hz.jqgfzy.top/gtiuballam.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hywenlv.cn/gtprwkyrpn.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtjcjbmmze.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hysaishi.cn/gtmbbgojfw.html

[Q68] 保存点
来源：http://hz.xuetiantiany.cn/gtrojwctjq.html

SAVEPOINT sp1;
来源：http://hz.jlsjyb.cn/gtrhxeilsh.html

ROLLBACK TO sp1;
来源：http://hz.yj202588.top/gtmhixxuqk.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtqcxhvwbj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.meibo888.top/gteapomfbk.html

[Q70] 更新统计信息
来源：http://hz.yangfankeji.com/gtkdqmpfjj.html

ANALYZE TABLE users;
来源：http://hz.sufxvd.cn/gtqylaknks.html

[Q71] 查看建表语句
来源：http://hz.ywan-chungtsiang.top/gtjuklurhi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.52xcode.cn/gtrxrrjsjp.html

[Q72] 查看索引
来源：http://hz.shangyingyoupin.top/gtdyuvoivl.html

SHOW INDEX FROM users;
来源：http://hz.feifeiyinyue.top/gtaucepfro.html

[Q73] 查看表状态
来源：http://hz.jinghuilouyu.cn/gteuxtqiay.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cqqwz.cn/gtqblivtxd.html

[Q74] 强制使用索引
来源：http://hz.yuxming.cn/gtfyblbtzb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhixingplan.top/gtielbshxw.html

[Q75] 日期格式化
来源：http://hz.cheryme.top/gtuqdyazyp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj20258888.top/gtkltgdser.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guannengcc.top/gtnykhiryr.html

[Q76] 按天统计
来源：http://hz.9152youxi.cn/gttjnbnqqr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dashuyun.cn/gtmvvgndiq.html

[Q77] 时间加减
来源：http://hz.hysaishi.cn/gtbmpinott.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydjk.org.cn/gtovkgzeal.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtiiotwvxf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hongshengwenyu.top/gtxdxgjpsa.html

[Q79] 字符串拼接
来源：http://hz.bjfxy.top/gtcenddpku.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.quarkkingdee.top/gtxrdictlg.html

[Q80] 字符串截取
来源：http://hz.zhaomingkeji.xyz/gtxikctdfp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zycfv.cn/gtjopbwmfv.html

[Q81] 字符串替换
来源：http://hz.hongshengwenyu.top/gtelqgwmfc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.smart0.xyz/gtmwerwcqy.html

[Q82] 字符长度与字节长度
来源：http://hz.shanyushiyangkeji.top/gtrsojgmld.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.iojbl.cn/gtzuesmihs.html

[Q83] 大小写转换
来源：http://hz.jianghu66.top/gtxvipnwzu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtpiepprwz.html

[Q84] 去除首尾空格
来源：http://hz.zhixingplan.top/gtpnqobcyx.html

SELECT TRIM(name) FROM users;
来源：http://hz.jyoumei.cn/gtvzlofoxo.html

[Q85] 数值取整
来源：http://hz.zhiwuduotai.top/gtywoxneft.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj20258888.top/gthvxmckzh.html

[Q86] 读取 JSON 字段
来源：http://hz.yuanzhike.top/gtoextyawe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.snrcjt.cn/gtziovdead.html

[Q87] JSON 字段做条件
来源：http://hz.zhixingplan.top/gtdgjbpmlo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cucudq.cn/gtuhijzcay.html

[Q88] 行转列（条件聚合）
来源：http://hz.yanxiufei.cn/gttpeznnnv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zdqjudy.top/gtgezgnfmm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hammf.cn/gtjmcihjtl.html

[Q89] 判断表是否存在
来源：http://hz.gogol.net.cn/gtdlukuvei.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258.top/gtsvewavel.html

[Q90] 生成序号列
来源：http://hz.hnxiangtu.top/gteojkdbkj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.andypj.xyz/gtqvuhvimu.html

================================================================================
来源：http://hz.redwolf501.top/gthcmsyijk.html

R. Bash 专题
来源：http://hz.zhiwuduotai.top/gtpfdkfafb.html

================================================================================
来源：http://hz.zycfv.cn/gtxzvirqwv.html

[R01] shebang 与严格模式
来源：http://hz.yj202588.top/gtvpuekjno.html

#!/usr/bin/env bash
来源：http://hz.sxryk.cn/gtnomzqdko.html

set -euo pipefail
来源：http://hz.cheryme.top/gtrudtabkl.html

[R02] 变量赋值与使用
来源：http://hz.smart0.xyz/gttyicytgj.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gtoxbojygr.html

[R03] 只读变量
来源：http://hz.zhijiandao.cn/gtzuynzfvz.html

readonly PI=3.14
来源：http://hz.hammf.cn/gtycvyiltm.html

[R04] 位置参数
来源：http://hz.zhoulong.xyz/gtgjiaoaja.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhijiandao.cn/gtruooaxmg.html

[R05] 参数默认值
来源：http://hz.smart0.xyz/gtvxcdumwq.html

name="${1:-default}"
来源：http://hz.jinqigufen.top/gtbjkufcoc.html

[R06] 判断命令是否存在
来源：http://hz.sweek.top/gttmkorqzk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aibaodan.cn/gtzyyxahfb.html

[R07] if 判断文件
来源：http://hz.yangfankeji.com/gtpzidieuu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigfzy.top/gtwpzttdjb.html

[R08] 数值比较
来源：http://hz.quarkkingdee.top/gtumghtyrj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cucudq.cn/gtgggpbdpz.html

[R09] 字符串比较
来源：http://hz.jinqigfzy.top/gtlhlessyd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shuidangran.top/gtaxlvdyqj.html

[R10] 正则匹配
来源：http://hz.nanxuanxn.top/gtbzotcelv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hywenlv.cn/gterjbduel.html

[R11] case 多分支
来源：http://hz.dianchejie.cn/gtnlcqaczr.html

case "$1" in
来源：http://hz.snrcjt.cn/gtlmeffaxk.html

start) echo "启动" ;;
来源：http://hz.sxryk.cn/gtrtkrleco.html

stop)  echo "停止" ;;
来源：http://hz.shuidangran.top/gtlmrgixlz.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtsfxvvapj.html

esac
来源：http://hz.chenzaomai.com/gtrplspnqs.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangtech.top/gtxjxktymm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.meibo888.top/gtrrizheva.html

[R13] for 计数循环
来源：http://hz.fengsongda.top/gtmtlbbjsq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtvulpvujx.html

[R14] C 风格 for
来源：http://hz.yonumen.top/gtiijohkqa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gtrmolqyzs.html

[R15] while 逐行读文件
来源：http://hz.nanxinkj.top/gtspljnqgs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ybcxt.top/gtjazphsav.html

[R16] until 等待条件
来源：http://hz.yongpay.top/gtdjjjkltk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj20258888.top/gtvgwhcnah.html

[R17] 数组定义与取值
来源：http://hz.jinyuanbaomall.cn/gtbszaxvns.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nwbrower.top/gtlbpapjep.html

[R18] 遍历数组
来源：http://hz.zhongyouzk.top/gtpzhilkei.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtuqnjhpie.html

[R19] 数组长度
来源：http://hz.jinqigufen.top/gtlnkniqvi.html

echo "${#arr[@]}"
来源：http://hz.hfpthk.cn/gtxviwhslm.html

[R20] 关联数组（字典）
来源：http://hz.shangyingyoupin.top/gtlsystcxz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sweek.top/gtqwilweco.html

[R21] 字符串长度
来源：http://hz.quarkkingdee.top/gtamapqrcw.html

echo "${#s}"
来源：http://hz.zhengqikj.top/gtoyhnckiv.html

[R22] 截取子串
来源：http://hz.316326.xyz/gtzhssgjkk.html

echo "${s:0:5}"
来源：http://hz.sysykeji.top/gtatpnhlna.html

[R23] 字符串替换
来源：http://hz.yj20258.top/gtmvtstkcc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhaomingkeji.xyz/gthafijglj.html

[R24] 大小写转换
来源：http://hz.zdqjudy.top/gtiaruvkkw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yongpay.top/gtwwljuxot.html

[R25] 去后缀 / 去前缀
来源：http://hz.feifeiyinyue.top/gtlkocymts.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.pengpengdd.cyou/gtwsnluxid.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtlwckgsiq.html

now=$(date +%F); echo "$now"
来源：http://hz.shangyingyoupin.top/gttkftvdul.html

[R27] 算术展开
来源：http://hz.hnqzz.top/gtoyenerah.html

echo $((1 + 2 * 3))
来源：http://hz.shzxlz.cn/gtlnlvcwse.html

[R28] 浮点运算
来源：http://hz.yj20258.top/gtagwdzhtf.html

echo "scale=2; 10/3" | bc
来源：http://hz.hywenlv.cn/gtwotbeqti.html

[R29] 定义函数
来源：http://hz.chenlongwang.top/gtlcprsesu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.havefunace.top/gttvjecjwc.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtebndhluk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cdnleiting.top/gtevbfrxcu.html

[R31] 局部变量
来源：http://hz.yangfankeji.com/gtorcqjswp.html

f() { local x=1; echo "$x"; }
来源：http://hz.shangyingyoupin.top/gtdfwgfqlq.html

[R32] 参数个数校验
来源：http://hz.sxryk.cn/gtregqnkva.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenlongwang.top/gtmfcrbsyi.html

[R33] 捕获错误并提示行号
来源：http://hz.9152youxi.cn/gticxmhxfy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj202588.top/gtpdzndxnh.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gtdlchobrq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtyofziybe.html

[R35] 后台执行并等待
来源：http://hz.nanxinkj.top/gtkoxfdkkg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuanzx.com/gtkhujrfwk.html

[R36] 并发执行多个任务
来源：http://hz.yj20258888.top/gtpvfwvwoh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj202588.top/gtcermgjmd.html

[R37] 把输出赋给变量
来源：http://hz.0kj1m.cn/gthqullzqm.html

files=$(ls -1)
来源：http://hz.iojbl.cn/gtzmdpsetv.html

[R38] 管道串联
来源：http://hz.shangyingyoupin.top/gtbygdeixm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tian-w.cn/gtfcwilfit.html

[R39] 重定向标准输出与错误
来源：http://hz.xziqi.cn/gtyqokdvmo.html

cmd > out.log 2>&1
来源：http://hz.guannengcc.top/gtsldnpcsv.html

[R40] 追加写日志
来源：http://hz.quarkkingdee.top/gthldrmfml.html

echo "log" >> out.log
来源：http://hz.hammf.cn/gtqmjoqrja.html

[R41] 丢弃输出
来源：http://hz.shzxlz.cn/gthrkqvdby.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigufen.top/gtsmpmyqsl.html

[R42] 输入重定向
来源：http://hz.yvedp.cn/gtgvlskatv.html

wc -l < a.txt
来源：http://hz.ivvv.top/gtnnlaziqv.html

[R43] 按名字查找文件
来源：http://hz.tanke756.top/gtrasdcnkd.html

find . -name "*.log" -type f
来源：http://hz.gzhubu.top/gtuvdoecms.html

[R44] 按修改时间查找
来源：http://hz.zhengqikj.top/gtdcipizjb.html

find . -mtime -7 -type f
来源：http://hz.sysykeji.top/gtaicvpbrq.html

[R45] 批量删除
来源：http://hz.ivvv.top/gtizeqjizd.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangtech.top/gtbtwgttrk.html

[R46] 递归替换文件内容
来源：http://hz.yj20258.top/gtvleeiili.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hfpthk.cn/gtyivwzoen.html

[R47] sed 单行替换
来源：http://hz.shuidangran.top/gtlovhazbk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxinkj.top/gtiallcpmg.html

[R48] awk 取指定列
来源：http://hz.jqgfzy.top/gtwjohptgf.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnqzz.top/gtuzqipauc.html

[R49] awk 带条件
来源：http://hz.jlsjyb.cn/gtxsvgjadw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangdashe.top/gtkxppsqyr.html

[R50] awk 求和
来源：http://hz.52xcode.cn/gtcqvfvoqc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.52xcode.cn/gtdmbexvty.html

[R51] 排序去重取前几
来源：http://hz.ivvv.top/gtstpcwqez.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jlsjyb.cn/gtjsyjzzbc.html

[R52] 统计行数
来源：http://hz.zhengqikj.top/gtxlxzfzws.html

wc -l a.txt
来源：http://hz.ehwqpu.com/gtrkqzjsok.html

[R53] 查看文件头与实时尾
来源：http://hz.ydjk.org.cn/gtqgtzfyqm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aibaodan.cn/gtryhbziug.html

[R54] 比较两个文件
来源：http://hz.ydjk.org.cn/gtfrnvjpai.html

diff a.txt b.txt
来源：http://hz.yanxiufei.cn/gtoeyavhjd.html

[R55] 压缩与解压
来源：http://hz.meibo888.top/gtqzxnbajo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.9152youxi.cn/gtpkupouli.html

[R56] 远程拷贝
来源：http://hz.gogol.net.cn/gtahbphvwl.html

scp file user@host:/path/
来源：http://hz.havefunace.top/gtpipqafhs.html

[R57] 远程执行命令
来源：http://hz.zhongyouzk.top/gttqgnkdlw.html

ssh user@host 'uptime'
来源：http://hz.feifeiyinyue.top/gtbuclyqlg.html

[R58] 下载文件
来源：http://hz.haohaochexian.top/gtdlrthumc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yuanzhike.top/gtxwcdnjwj.html

[R59] 发 POST JSON
来源：http://hz.nwbrower.top/gtyvhzydwf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhixingplan.top/gtqiwmmmsh.html

[R60] 只看 HTTP 状态码
来源：http://hz.jyoumei.cn/gtwgxxezzq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhoulong.xyz/gtkewjezwi.html

[R61] 磁盘占用
来源：http://hz.fengsongda.top/gtcxfngcnw.html

df -h;  du -sh *
来源：http://hz.gotoacloud.top/gtcigltugl.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtpcvsznas.html

du -ah . | sort -rh | head -10
来源：http://hz.ehwqpu.com/gthqzqvvwe.html

[R63] 内存与进程
来源：http://hz.gogol.net.cn/gtrdijcvqg.html

free -h;  ps aux | grep nginx
来源：http://hz.ywan-chungtsiang.top/gtcikhsocy.html

[R64] 结束进程
来源：http://hz.xingfuxueyuan.xyz/gthaiyyyjn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.iojbl.cn/gtiuvdcevx.html

[R65] 查看端口占用
来源：http://hz.0kj1m.cn/gtrmcxdubo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xuetiantiany.cn/gtyotvicdm.html

[R66] 定时任务
来源：http://hz.316326.xyz/gttgbzqacb.html

crontab -e;  crontab -l
来源：http://hz.jinghuilouyu.cn/gttybrnuiq.html

[R67] 生成随机十六进制串
来源：http://hz.yonumen.top/gtgmskgcbu.html

openssl rand -hex 16
来源：http://hz.sufxvd.cn/gtgigindas.html

[R68] 计算文件校验值
来源：http://hz.shzxlz.cn/gtanwogsfa.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yongpay.top/gtdoctmgco.html

[R69] 生成随机密码
来源：http://hz.gaohongyu789.top/gtzojtgsyb.html

head -c 16 /dev/urandom | base64
来源：http://hz.yangfankeji.com/gtcsytqfgf.html

[R70] 时间戳与互转
来源：http://hz.birdmap.top/gtpxhakiex.html

date +%s;  date -d @1700000000
来源：http://hz.ybcxt.top/gtrnylylfi.html

[R71] 日期格式化
来源：http://hz.shangyingyoupin.top/gtduaxmiib.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnqzz.top/gtbqciofma.html

[R72] 等待端口就绪
来源：http://hz.feifeiyinyue.top/gtrdixpcri.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhengqikj.top/gtethxnzbc.html

[R73] 分割大日志
来源：http://hz.zdqjudy.top/gtfzaclmei.html

split -l 1000 big.log part_
来源：http://hz.shzxlz.cn/gtvkqoodzg.html

[R74] 批量重命名
来源：http://hz.9152youxi.cn/gtzryeqfum.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cdnleiting.top/gtdtnutfiu.html

[R75] 导出环境变量
来源：http://hz.zhixingplan.top/gttwrruvgn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhiwuduotai.top/gtfzflgrzi.html

[R76] 使用临时文件
来源：http://hz.cashguo.top/gtkmbwpwgo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.smart0.xyz/gtbikapbyy.html

[R77] 读取用户输入
来源：http://hz.yj202588.top/gteavuetql.html

read -rp "请输入: " ans
来源：http://hz.zhixingplan.top/gtvcvzasba.html

[R78] 交互式菜单
来源：http://hz.sxryk.cn/gtuelnpvik.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.316326.xyz/gtgbcdzpyc.html

[R79] 解析命令行选项
来源：http://hz.iojbl.cn/gtrawvoxel.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.mhx1999.top/gtoqcaqlqw.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtvgcvtnhh.html

time ./run.sh
来源：http://hz.aizwys.cn/gtijzqkijm.html

================================================================================
来源：http://hz.0kj1m.cn/gtdulzaoik.html

S. C / C++ 专题
来源：http://hz.wangdashe.top/gtrnklbzaj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtvkwxxvtc.html

[S01] C：Hello World
来源：http://hz.ydzc1.top/gtpccqufmh.html

#include <stdio.h>
来源：http://hz.ivvv.top/gtybocwpsr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fengsongda.top/gtbnzbtblm.html

[S02] C：变量与格式化输出
来源：http://hz.haohaochexian.top/gticclbxqc.html

int a = 10; printf("%d\n", a);
来源：http://hz.xylfe.cn/gtomfjhvnd.html

[S03] C：读入整数
来源：http://hz.wangdashe.top/gtyrcueinr.html

int x; scanf("%d", &x);
来源：http://hz.ehwqpu.com/gtfjthdjhh.html

[S04] C：字符串复制
来源：http://hz.birdmap.top/gtzzgsvkan.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.snrcjt.cn/gtyircorhe.html

[S05] C：字符串长度
来源：http://hz.jinyuanbaomall.cn/gtbcpzdskr.html

strlen(s)
来源：http://hz.hnqzz.top/gthbfbcbtd.html

[S06] C：字符串比较
来源：http://hz.yvedp.cn/gtdxcszjxm.html

strcmp(a, b) == 0
来源：http://hz.jqgufenzy.top/gtyevwrqdc.html

[S07] C：数组遍历求和
来源：http://hz.redwolf501.top/gtvoeskayt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.c1oappe.top/gtoonmllyw.html

[S08] C：动态内存分配与释放
来源：http://hz.yongpay.top/gteullhfuu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj202588.top/gtkvyhbgcv.html

[S09] C：结构体定义与初始化
来源：http://hz.kuanghao11.cn/gtljxqiwkl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhengqikj.top/gtgnqqexei.html

[S10] C：指针与解引用
来源：http://hz.xziqi.cn/gtvgaxohrm.html

int *p = &a;  *p = 5;
来源：http://hz.9152youxi.cn/gtogjiycxl.html

[S11] C：逐行读文件
来源：http://hz.smart0.xyz/gtqevifijt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigufen.top/gtqofoyrnc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhoulong.xyz/gtojspehya.html

fclose(f);
来源：http://hz.hfpthk.cn/gtvshgajnd.html

[S12] C：写文件
来源：http://hz.wangdashe.top/gtpyczgicx.html


<!-- 参考信息 -->