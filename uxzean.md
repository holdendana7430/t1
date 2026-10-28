代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.316326.xyz/gtwmonzxub.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jqgufenzy.top/gtcffdpnbq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jiagoushi.top/gtjshkakzd.html

[Q42] 连接条件附加过滤
来源：http://hz.cqqwz.cn/gtvqfkfxbf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nwbrower.top/gtkrsdxtii.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinghuilouyu.cn/gtpxmrgvex.html

[Q43] 标量子查询
来源：http://hz.zhiwuduotai.top/gtabysmeid.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydjk.org.cn/gtlbhenynf.html

[Q44] IN 子查询
来源：http://hz.yueranfly.top/gtazyiwiuc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shuidangran.top/gtvzdkglkp.html

[Q45] EXISTS 判断存在
来源：http://hz.vqdsnc.cn/gtszzmvmia.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtnmxbxwac.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jyoumei.cn/gtvtjjchin.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.52xcode.cn/gtwwgwarek.html

[Q47] 与平均值比较
来源：http://hz.yanxiufei.cn/gtxwggbsif.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydjk.org.cn/gtwgdndhro.html

[Q48] CTE 公用表表达式
来源：http://hz.chenjidiqi.icu/gtqespetmc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.mhx1999.top/gtdidoyjnq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fzhhl.top/gtyndovkaw.html

[Q49] 更新单行
来源：http://hz.chenzaomai.com/gtmqyixpum.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tanke756.top/gtcwhzcqwe.html

[Q50] 批量更新
来源：http://hz.bjfxy.top/gtgtjxozom.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhongyouzk.top/gtuhuadcgj.html

[Q51] 用子查询更新
来源：http://hz.nwbrower.top/gtkkbiptvk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sufxvd.cn/gtjbuyttls.html

[Q52] 删除指定行
来源：http://hz.zhiwuduotai.top/gtraemsgko.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nanxuanxn.top/gtprxxswee.html

[Q53] 按条件删除
来源：http://hz.zhengqikj.top/gtgojzrqch.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.haohaochexian.top/gtydswlczd.html

[Q54] 清空表
来源：http://hz.fengsongda.top/gtjkzhcjfk.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258.top/gtkdnelnpr.html

[Q55] 排名（并列占位）
来源：http://hz.yonumen.top/gtwiirizhr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shzxlz.cn/gtjolhdgef.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yonumen.top/gtlkelrhzm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.fengsongda.top/gtdxccohhb.html

[Q57] 行号
来源：http://hz.iojbl.cn/gtjtooiker.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj20258.top/gtlcwodach.html

[Q58] 累计求和
来源：http://hz.yj202588.top/gtcyxoecmi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yongpay.top/gtyoajidqi.html

[Q59] 分组内累计
来源：http://hz.ywan-chungtsiang.top/gtejgqwskw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.feifeiyinyue.top/gtgzuahnrc.html

[Q60] 取上一行 / 下一行
来源：http://hz.yangfankeji.com/gtbtukfban.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sxryk.cn/gtbnvhasag.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sweek.top/gtpngihoul.html

[Q61] 移动平均
来源：http://hz.bjfxy.top/gthlurjsfw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yonumen.top/gtstjclwdw.html

[Q62] 分组占比
来源：http://hz.xinyue.icu/gtodggjcdh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtaxykqenq.html

[Q63] 开启事务
来源：http://hz.zhengqikj.top/gtjkgweqii.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuxming.cn/gtcppgoihp.html

[Q64] 提交事务
来源：http://hz.xziqi.cn/gtipptoiuu.html

COMMIT;
来源：http://hz.hammf.cn/gtvdudaynq.html

[Q65] 回滚事务
来源：http://hz.zhijiandao.cn/gtgsfdzjzw.html

ROLLBACK;
来源：http://hz.hammf.cn/gtfteccxoo.html

[Q66] 行锁查询
来源：http://hz.mhx1999.top/gtlpsuacho.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenzaomai.com/gtjdmierlv.html

[Q67] 设置隔离级别
来源：http://hz.hywenlv.cn/gtiguzszus.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinghuilouyu.cn/gtnbhjqfbh.html

[Q68] 保存点
来源：http://hz.kuanghao11.cn/gtwajgsoma.html

SAVEPOINT sp1;
来源：http://hz.tian-w.cn/gtieehlewo.html

ROLLBACK TO sp1;
来源：http://hz.hongshengwenyu.top/gtbrqlofot.html

[Q69] 查看执行计划
来源：http://hz.ywan-chungtsiang.top/gtmjidziqo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgfzy.top/gtljbbclmb.html

[Q70] 更新统计信息
来源：http://hz.cdnleiting.top/gtewoszwng.html

ANALYZE TABLE users;
来源：http://hz.guowangkeji.top/gteqjsnecl.html

[Q71] 查看建表语句
来源：http://hz.nanxinkj.top/gtkpthvynu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ivvv.top/gtvsbclbfw.html

[Q72] 查看索引
来源：http://hz.yanxiufei.cn/gtpwuhrrnr.html

SHOW INDEX FROM users;
来源：http://hz.chenzaomai.com/gteloniocs.html

[Q73] 查看表状态
来源：http://hz.yanxiufei.cn/gtihedndrv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jlsjyb.cn/gtcgxbeceu.html

[Q74] 强制使用索引
来源：http://hz.jinghuilouyu.cn/gtracpkyfb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuanzx.com/gtyawkjdht.html

[Q75] 日期格式化
来源：http://hz.ehwqpu.com/gthlkcnuvg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinqigufen.top/gttlqtqxhr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.mhx1999.top/gtofpjajln.html

[Q76] 按天统计
来源：http://hz.9152youxi.cn/gtlctvlytn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.52xcode.cn/gtiggdgeov.html

[Q77] 时间加减
来源：http://hz.iojbl.cn/gtocqajwuz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgfzy.top/gtwymhbura.html

[Q78] 当前时间
来源：http://hz.shuidangran.top/gtgqeijlbz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dashuyun.cn/gtfnjccgce.html

[Q79] 字符串拼接
来源：http://hz.yj20258888.top/gtlcsytrdj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cheryme.top/gtrgitztpm.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangkeji.top/gtjrmghbzl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hnqzz.top/gtgxcfiweq.html

[Q81] 字符串替换
来源：http://hz.gogol.net.cn/gtkrubujav.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shzxlz.cn/gtqsihpwfz.html

[Q82] 字符长度与字节长度
来源：http://hz.jqgufenzy.top/gteralmkqb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sweek.top/gtirdpmlye.html

[Q83] 大小写转换
来源：http://hz.mhx1999.top/gtuomlcncz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jiagoushi.top/gtmpkqxbbx.html

[Q84] 去除首尾空格
来源：http://hz.chenlongwang.top/gtulyecxnb.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtbbezuaia.html

[Q85] 数值取整
来源：http://hz.nwbrower.top/gtbvudxsbs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhijiandao.cn/gtbvcofziw.html

[Q86] 读取 JSON 字段
来源：http://hz.c1oappe.top/gtigmgqihi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sysykeji.top/gtytkbmrdd.html

[Q87] JSON 字段做条件
来源：http://hz.yj20258888.top/gtnxvblpup.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hammf.cn/gtjlizpjei.html

[Q88] 行转列（条件聚合）
来源：http://hz.zycfv.cn/gtonajrapa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tian-w.cn/gtvtxprzyu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.meibo888.top/gtgjxzrgwo.html

[Q89] 判断表是否存在
来源：http://hz.tanke756.top/gtrpfzitoe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yueranfly.top/gtllbuagbc.html

[Q90] 生成序号列
来源：http://hz.chenlongwang.top/gttafycpcj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenjidiqi.icu/gtwiysncdh.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtvbrglbsr.html

R. Bash 专题
来源：http://hz.redwolf501.top/gtyjanexkp.html

================================================================================
来源：http://hz.bjfxy.top/gtbgxwzhtg.html

[R01] shebang 与严格模式
来源：http://hz.ppjwa.cn/gtsgrwimha.html

#!/usr/bin/env bash
来源：http://hz.hywenlv.cn/gthbqwzlbf.html

set -euo pipefail
来源：http://hz.xziqi.cn/gtszzgotof.html

[R02] 变量赋值与使用
来源：http://hz.hfpthk.cn/gtfoxtvsaw.html

name="Tom"; echo "$name"
来源：http://hz.jqgfzy.top/gtaeqmeahe.html

[R03] 只读变量
来源：http://hz.bjfxy.top/gtcquvmies.html

readonly PI=3.14
来源：http://hz.yangfankeji.com/gtdilllhue.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gtciefjjti.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.quarkkingdee.top/gtavrdtowv.html

[R05] 参数默认值
来源：http://hz.chenzaomai.com/gtczpilrut.html

name="${1:-default}"
来源：http://hz.jqgfzy.top/gthjordtyc.html

[R06] 判断命令是否存在
来源：http://hz.shangyingyoupin.top/gthwzypdzn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jianghu66.top/gtpxsjkdsz.html

[R07] if 判断文件
来源：http://hz.jqgfzy.top/gtsofpyfiu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xylfe.cn/gtcuvvhkpb.html

[R08] 数值比较
来源：http://hz.gaohongyu789.top/gtqkqecssz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jianghu66.top/gtgywjkyqy.html

[R09] 字符串比较
来源：http://hz.quarkkingdee.top/gtycpwcacs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuanzhike.top/gtcmwvlpyk.html

[R10] 正则匹配
来源：http://hz.cucudq.cn/gtwncytejj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgfzy.top/gtezwitxmy.html

[R11] case 多分支
来源：http://hz.xylfe.cn/gthmaqcnyk.html

case "$1" in
来源：http://hz.yvedp.cn/gttqobmglv.html

start) echo "启动" ;;
来源：http://hz.sysykeji.top/gtymwhjygb.html

stop)  echo "停止" ;;
来源：http://hz.jqgfzy.top/gtoljmeffs.html

*)     echo "未知命令" ;;
来源：http://hz.kuanghao11.cn/gtzpkwhicl.html

esac
来源：http://hz.jqgfzy.top/gtelpugckc.html

[R12] for 遍历文件
来源：http://hz.ywan-chungtsiang.top/gtevilezcc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sweek.top/gtevwvxddz.html

[R13] for 计数循环
来源：http://hz.feifeiyinyue.top/gtcbrqfotn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuanzx.com/gtprulyrsk.html

[R14] C 风格 for
来源：http://hz.chenzaomai.com/gtkjsjdjtk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daxiang520.top/gtlmzzsyqz.html

[R15] while 逐行读文件
来源：http://hz.aizwys.cn/gtyonzmaqc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hysaishi.cn/gtozoawymf.html

[R16] until 等待条件
来源：http://hz.sysykeji.top/gtktfcwvuu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shzxlz.cn/gtlguifpov.html

[R17] 数组定义与取值
来源：http://hz.sufxvd.cn/gtkknaqktz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.316326.xyz/gtxzqpbxcl.html

[R18] 遍历数组
来源：http://hz.316326.xyz/gtqgfnpuae.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangshuangyany.cn/gtbyfjjwmh.html

[R19] 数组长度
来源：http://hz.9152youxi.cn/gtrqtgsgsu.html

echo "${#arr[@]}"
来源：http://hz.shuidangran.top/gtcqbclxvq.html

[R20] 关联数组（字典）
来源：http://hz.jinghuilouyu.cn/gtvpiiwfkr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtbgifgtes.html

[R21] 字符串长度
来源：http://hz.hongshengwenyu.top/gtysbuanok.html

echo "${#s}"
来源：http://hz.xziqi.cn/gtogrhkdgg.html

[R22] 截取子串
来源：http://hz.yonumen.top/gtxvfbuewi.html

echo "${s:0:5}"
来源：http://hz.havefunace.top/gttwsxpnbw.html

[R23] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtttxcpbjj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.0kj1m.cn/gtvvmdngce.html

[R24] 大小写转换
来源：http://hz.ppjwa.cn/gtbizvbbza.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ybcxt.top/gtsclkiwsp.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhoulong.xyz/gtjglayxbu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuetiantiany.cn/gtarkphfxx.html

[R26] 命令替换
来源：http://hz.jinghuilouyu.cn/gtvrscpdtv.html

now=$(date +%F); echo "$now"
来源：http://hz.hywenlv.cn/gtntuvkgyf.html

[R27] 算术展开
来源：http://hz.pycfn.com/gtnolkdesy.html

echo $((1 + 2 * 3))
来源：http://hz.yvedp.cn/gttwuoaktc.html

[R28] 浮点运算
来源：http://hz.zhongyouzk.top/gtvzfmasax.html

echo "scale=2; 10/3" | bc
来源：http://hz.yanxiufei.cn/gtgqsgomun.html

[R29] 定义函数
来源：http://hz.hongshengwenyu.top/gtproduked.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xingfuxueyuan.xyz/gthbdxgruc.html

[R30] 函数返回状态码
来源：http://hz.tanke756.top/gtggpieiva.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cheryme.top/gtzflmkucv.html

[R31] 局部变量
来源：http://hz.guannengcc.top/gtpurmdvda.html

f() { local x=1; echo "$x"; }
来源：http://hz.gaohongyu789.top/gtncibjbhh.html

[R32] 参数个数校验
来源：http://hz.xuetiantiany.cn/gtgwbcufuu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhongyouzk.top/gtkmtemofi.html

[R33] 捕获错误并提示行号
来源：http://hz.wangshuangyany.cn/gtaiqpsefx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangkeji.top/gtgacketpa.html

[R34] 退出时清理
来源：http://hz.yonumen.top/gtaogxylge.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.c1oappe.top/gtjfykeidx.html

[R35] 后台执行并等待
来源：http://hz.cqqwz.cn/gthchtyqxn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yueranfly.top/gtruznrtpq.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtkljiibkl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.smart0.xyz/gtrvmpeuxl.html

[R37] 把输出赋给变量
来源：http://hz.yongpay.top/gtrdbuqwck.html

files=$(ls -1)
来源：http://hz.redwolf501.top/gtkdnizqju.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtluhnryof.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jyoumei.cn/gtxjrrpuuv.html

[R39] 重定向标准输出与错误
来源：http://hz.aibaodan.cn/gtilfzxrlb.html

cmd > out.log 2>&1
来源：http://hz.fzhhl.top/gtlrxvppcw.html

[R40] 追加写日志
来源：http://hz.ywan-chungtsiang.top/gtwlznrcju.html

echo "log" >> out.log
来源：http://hz.52xcode.cn/gtlkbbvuni.html

[R41] 丢弃输出
来源：http://hz.cucudq.cn/gtbafmhpme.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gtovmptwev.html

[R42] 输入重定向
来源：http://hz.sufxvd.cn/gtdqnnbvmn.html

wc -l < a.txt
来源：http://hz.havefunace.top/gtnwlotyew.html

[R43] 按名字查找文件
来源：http://hz.birdmap.top/gtmalwmzpk.html

find . -name "*.log" -type f
来源：http://hz.jqgufenzy.top/gtshngxcqa.html

[R44] 按修改时间查找
来源：http://hz.tanke756.top/gtzgfijtob.html

find . -mtime -7 -type f
来源：http://hz.chenjidiqi.icu/gtfrfwigng.html

[R45] 批量删除
来源：http://hz.havefunace.top/gtdstyehew.html

find . -name "*.tmp" -delete
来源：http://hz.birdmap.top/gtmwqumwjc.html

[R46] 递归替换文件内容
来源：http://hz.aizwys.cn/gtorifgoap.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ydzc1.top/gtzjgirwth.html

[R47] sed 单行替换
来源：http://hz.aibaodan.cn/gtdiwxikts.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jiagoushi.top/gtudcojocp.html

[R48] awk 取指定列
来源：http://hz.jyoumei.cn/gtrlzktdzr.html

awk '{print $1, $3}' a.txt
来源：http://hz.0kj1m.cn/gtwbvdqnke.html

[R49] awk 带条件
来源：http://hz.hfpthk.cn/gtmebhhbkh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ywan-chungtsiang.top/gtnqfghhhg.html

[R50] awk 求和
来源：http://hz.iojbl.cn/gtxsuzvysh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.haohaochexian.top/gttnuqqsiv.html

[R51] 排序去重取前几
来源：http://hz.hysaishi.cn/gtzquyhvja.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258888.top/gthluhepqu.html

[R52] 统计行数
来源：http://hz.yanxiufei.cn/gtfhhgtkva.html

wc -l a.txt
来源：http://hz.yueranfly.top/gtywfezcog.html

[R53] 查看文件头与实时尾
来源：http://hz.gogol.net.cn/gtcllkjxjy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhijiandao.cn/gthrranpuj.html

[R54] 比较两个文件
来源：http://hz.snrcjt.cn/gtvpnungve.html

diff a.txt b.txt
来源：http://hz.zhiwuduotai.top/gtpntgueij.html

[R55] 压缩与解压
来源：http://hz.meibo888.top/gtjfnkzgtf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gogol.net.cn/gtgdhpmzzd.html

[R56] 远程拷贝
来源：http://hz.guowangkeji.top/gtqzlptank.html

scp file user@host:/path/
来源：http://hz.gaohongyu789.top/gtdumbcgml.html

[R57] 远程执行命令
来源：http://hz.hywenlv.cn/gtubgaltfs.html

ssh user@host 'uptime'
来源：http://hz.redwolf501.top/gtigckrgdq.html

[R58] 下载文件
来源：http://hz.chenjidiqi.icu/gtmkbafmoy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gaohongyu789.top/gtegscjpee.html

[R59] 发 POST JSON
来源：http://hz.nwbrower.top/gtbnpusulv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jyoumei.cn/gtfmdupusd.html

[R60] 只看 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtklgfzqwi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydzc1.top/gthyzltklu.html

[R61] 磁盘占用
来源：http://hz.jinqigfzy.top/gtnhzsevcq.html

df -h;  du -sh *
来源：http://hz.kuanghao11.cn/gthblgiuoc.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtybupiaxn.html

du -ah . | sort -rh | head -10
来源：http://hz.sxryk.cn/gtwttdxozy.html

[R63] 内存与进程
来源：http://hz.hysaishi.cn/gtaxbvtyqi.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258888.top/gtszfsihrk.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtwpptqjza.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtxbupjuug.html

[R65] 查看端口占用
来源：http://hz.mhx1999.top/gtpduttipw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinghuilouyu.cn/gttjrebhlk.html

[R66] 定时任务
来源：http://hz.zycfv.cn/gtngpyhvzs.html

crontab -e;  crontab -l
来源：http://hz.birdmap.top/gtgtsalhyu.html

[R67] 生成随机十六进制串
来源：http://hz.jlsjyb.cn/gtejuozhsh.html

openssl rand -hex 16
来源：http://hz.chenlongwang.top/gtdbjeoepq.html

[R68] 计算文件校验值
来源：http://hz.dianchejie.cn/gtqfsmmwta.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.9152youxi.cn/gtncgrbvxo.html

[R69] 生成随机密码
来源：http://hz.svipenyu.cn/gtzzwtcjjx.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxinkj.top/gtzrkjjcdf.html

[R70] 时间戳与互转
来源：http://hz.chenzaomai.com/gtvkesiksf.html

date +%s;  date -d @1700000000
来源：http://hz.cdnleiting.top/gtsvjndvgg.html

[R71] 日期格式化
来源：http://hz.gzhubu.top/gtxpcifoqx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sufxvd.cn/gtzijsmprl.html

[R72] 等待端口就绪
来源：http://hz.andypj.xyz/gtbyhcdvpu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gtlaqeyavi.html

[R73] 分割大日志
来源：http://hz.feifeiyinyue.top/gtympewbyx.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangkeji.top/gtfvevuhyb.html

[R74] 批量重命名
来源：http://hz.yj20258888.top/gtdicdttnw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtlregtvuh.html

[R75] 导出环境变量
来源：http://hz.jinyuanbaomall.cn/gtixcnreiz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinghuilouyu.cn/gtbgkghjjx.html

[R76] 使用临时文件
来源：http://hz.zhiwuduotai.top/gtictgteoy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dashuyun.cn/gtluzjoxor.html

[R77] 读取用户输入
来源：http://hz.jlsjyb.cn/gtouogawtl.html

read -rp "请输入: " ans
来源：http://hz.meibo888.top/gtsvisnhgd.html

[R78] 交互式菜单
来源：http://hz.316326.xyz/gtcsgbxfzs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinghuilouyu.cn/gtowddbqlj.html

[R79] 解析命令行选项
来源：http://hz.jinqigufen.top/gtbqbwatee.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinyuanbaomall.cn/gtkboegkor.html

[R80] 查看脚本执行耗时
来源：http://hz.smart0.xyz/gtvzgvyuxv.html

time ./run.sh
来源：http://hz.chenzaomai.com/gtqbgvhjup.html

================================================================================
来源：http://hz.svipenyu.cn/gtsvudslgi.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gtistretuu.html

================================================================================
来源：http://hz.shzxlz.cn/gtogdzmkrx.html

[S01] C：Hello World
来源：http://hz.pengpengdd.cyou/gtojqipsck.html

#include <stdio.h>
来源：http://hz.iojbl.cn/gtvkybzyvc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hfpthk.cn/gtxtoiovil.html

[S02] C：变量与格式化输出
来源：http://hz.c1oappe.top/gtheichbey.html

int a = 10; printf("%d\n", a);
来源：http://hz.sysykeji.top/gtpygdvzpe.html

[S03] C：读入整数
来源：http://hz.yuanzhike.top/gtyxtrntmc.html

int x; scanf("%d", &x);
来源：http://hz.shuidangran.top/gtowmkyioh.html

[S04] C：字符串复制
来源：http://hz.wangshuangyany.cn/gtsatibeaf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.redwolf501.top/gtqgyhxsdl.html

[S05] C：字符串长度
来源：http://hz.aizwys.cn/gtyogmgilp.html

strlen(s)
来源：http://hz.zhaomingkeji.xyz/gtxmcppdkd.html

[S06] C：字符串比较
来源：http://hz.chenjidiqi.icu/gtjytodxao.html

strcmp(a, b) == 0
来源：http://hz.redwolf501.top/gtqacwplha.html

[S07] C：数组遍历求和
来源：http://hz.shanyushiyangtech.top/gtviduebgy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sysykeji.top/gtcvhgixel.html

[S08] C：动态内存分配与释放
来源：http://hz.cashguo.top/gtqhhuthde.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pengpengdd.cyou/gtrzmoeukm.html

[S09] C：结构体定义与初始化
来源：http://hz.sysykeji.top/gtmmghfgaq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.c1oappe.top/gtugslzsaw.html

[S10] C：指针与解引用
来源：http://hz.guannengcc.top/gtybhozoxz.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigfzy.top/gtmbijxlly.html

[S11] C：逐行读文件
来源：http://hz.ydjk.org.cn/gtgmxlmros.html


<!-- 参考信息 -->