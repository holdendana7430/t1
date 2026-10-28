代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangkeji.top/gtscudsxqv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.0kj1m.cn/gtzrgtrtul.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhongyouzk.top/gthatmfbdn.html

[Q42] 连接条件附加过滤
来源：http://hz.gogol.net.cn/gtblargjio.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xingfuxueyuan.xyz/gtcmxauzuu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yangfankeji.com/gtaulsvnkb.html

[Q43] 标量子查询
来源：http://hz.9152youxi.cn/gtewspznuv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ybcxt.top/gtvlohwquf.html

[Q44] IN 子查询
来源：http://hz.svipenyu.cn/gtowawmmmu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hammf.cn/gtlkjodkfj.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258.top/gtvguhepqz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgfzy.top/gttusfejzg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhengqikj.top/gtakwzzwmp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtgbldehri.html

[Q47] 与平均值比较
来源：http://hz.ehwqpu.com/gtwzkymzrx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258888.top/gtxxmoogmo.html

[Q48] CTE 公用表表达式
来源：http://hz.cdnleiting.top/gtrchpjuqt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hywenlv.cn/gtinssvblr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ppjwa.cn/gtdvpgbrmq.html

[Q49] 更新单行
来源：http://hz.gotoacloud.top/gtjnvlhaok.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gotoacloud.top/gtoiuztxmt.html

[Q50] 批量更新
来源：http://hz.chenzaomai.com/gtwxnoerus.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sweek.top/gtzimwoeug.html

[Q51] 用子查询更新
来源：http://hz.yanxiufei.cn/gtijmbzvau.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gotoacloud.top/gtvinfrzdb.html

[Q52] 删除指定行
来源：http://hz.0kj1m.cn/gtczyltmkq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shzxlz.cn/gtjpuednzd.html

[Q53] 按条件删除
来源：http://hz.shanyushiyangtech.top/gtrfndzvfg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxinkj.top/gtgyzfegnj.html

[Q54] 清空表
来源：http://hz.bjfxy.top/gtlxncejap.html

TRUNCATE TABLE logs;
来源：http://hz.yuanzhike.top/gtqusmpnva.html

[Q55] 排名（并列占位）
来源：http://hz.jinqigfzy.top/gtsqhjwbyn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.guowangkeji.top/gtjznjixbw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.guowangkeji.top/gthebzyeqz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtssulhlbp.html

[Q57] 行号
来源：http://hz.0kj1m.cn/gthqepvieg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zdqjudy.top/gtedmewzml.html

[Q58] 累计求和
来源：http://hz.hywenlv.cn/gtlahmauoq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.vqdsnc.cn/gtdnvdsrcu.html

[Q59] 分组内累计
来源：http://hz.tianlin.xyz/gtlfnsgfri.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sxryk.cn/gtmlyphgzh.html

[Q60] 取上一行 / 下一行
来源：http://hz.svipenyu.cn/gtgrmoysck.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258888.top/gtihglbgrm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hfpthk.cn/gtaennvivd.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtvxpcyikm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtrfhybchr.html

[Q62] 分组占比
来源：http://hz.pycfn.com/gterxasvkp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtcsmfhddg.html

[Q63] 开启事务
来源：http://hz.cucudq.cn/gtpgvvmzmg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.dashuyun.cn/gtasscupch.html

[Q64] 提交事务
来源：http://hz.aizwys.cn/gtotlxvdos.html

COMMIT;
来源：http://hz.jinqigufen.top/gtiamxtkde.html

[Q65] 回滚事务
来源：http://hz.ybcxt.top/gtqhwricrs.html

ROLLBACK;
来源：http://hz.feifeiyinyue.top/gteoxyfqgn.html

[Q66] 行锁查询
来源：http://hz.gotoacloud.top/gtonczenxk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yvedp.cn/gtytdlstwm.html

[Q67] 设置隔离级别
来源：http://hz.redwolf501.top/gtpzprogtt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.52xcode.cn/gtlhastzvh.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtqvyrzcly.html

SAVEPOINT sp1;
来源：http://hz.aibaodan.cn/gtfysxnrzp.html

ROLLBACK TO sp1;
来源：http://hz.jlsjyb.cn/gtyplyqewg.html

[Q69] 查看执行计划
来源：http://hz.kuanghao11.cn/gtweqwjmol.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhoulong.xyz/gtjnacvlhx.html

[Q70] 更新统计信息
来源：http://hz.ppjwa.cn/gtkequcyba.html

ANALYZE TABLE users;
来源：http://hz.jqgfzy.top/gtzthyqdlz.html

[Q71] 查看建表语句
来源：http://hz.cashguo.top/gthsujkhxb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hongshengwenyu.top/gtlnotrxma.html

[Q72] 查看索引
来源：http://hz.smart0.xyz/gtatdfxnez.html

SHOW INDEX FROM users;
来源：http://hz.daxiang520.top/gtfoabkmcq.html

[Q73] 查看表状态
来源：http://hz.aizwys.cn/gtqzgyggqw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hywenlv.cn/gttklloqmy.html

[Q74] 强制使用索引
来源：http://hz.redwolf501.top/gtcnnlcxam.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xziqi.cn/gthhoilyvt.html

[Q75] 日期格式化
来源：http://hz.yangfankeji.com/gtzewuisxl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenjidiqi.icu/gtqpihueqi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ybcxt.top/gtdekzakve.html

[Q76] 按天统计
来源：http://hz.ivvv.top/gtivvkwjeb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hysaishi.cn/gtczsdlept.html

[Q77] 时间加减
来源：http://hz.yanxiufei.cn/gtccyjnvct.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuanzhike.top/gtrweyghuf.html

[Q78] 当前时间
来源：http://hz.hnqzz.top/gtezfsmabt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hysaishi.cn/gtkcknoaws.html

[Q79] 字符串拼接
来源：http://hz.zhongyouzk.top/gtzlomtnwc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shangyingyoupin.top/gtsmaevbtc.html

[Q80] 字符串截取
来源：http://hz.gogol.net.cn/gtwyebrnsf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.quarkkingdee.top/gtouqzvzff.html

[Q81] 字符串替换
来源：http://hz.snrcjt.cn/gtteyptuxo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.0kj1m.cn/gtkgvodxkv.html

[Q82] 字符长度与字节长度
来源：http://hz.chenlongwang.top/gtitzwrqjt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fzhhl.top/gtsbmafvnk.html

[Q83] 大小写转换
来源：http://hz.xylfe.cn/gtgovjubnn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zdqjudy.top/gtpqkzkoer.html

[Q84] 去除首尾空格
来源：http://hz.nanxinkj.top/gtrtzobufo.html

SELECT TRIM(name) FROM users;
来源：http://hz.svipenyu.cn/gtmmxmjndz.html

[Q85] 数值取整
来源：http://hz.gogol.net.cn/gteamuktxp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dashuyun.cn/gtbsxafwfc.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtzoxrdjhj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.iojbl.cn/gthpcziapu.html

[Q87] JSON 字段做条件
来源：http://hz.c1oappe.top/gtspudlpnr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258.top/gtkchfovom.html

[Q88] 行转列（条件聚合）
来源：http://hz.hammf.cn/gtxzfcyzle.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gotoacloud.top/gtoqwwpvuc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xziqi.cn/gtwbkymwdf.html

[Q89] 判断表是否存在
来源：http://hz.zhaomingkeji.xyz/gtbhrxlqmn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gaohongyu789.top/gtmcredcpu.html

[Q90] 生成序号列
来源：http://hz.xuetiantiany.cn/gtnpzzjhoa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shangyingyoupin.top/gtciqvtnvm.html

================================================================================
来源：http://hz.vqdsnc.cn/gtcevjaarz.html

R. Bash 专题
来源：http://hz.svipenyu.cn/gtjkusjdam.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtxocmggva.html

[R01] shebang 与严格模式
来源：http://hz.shangyingyoupin.top/gtviqsuyga.html

#!/usr/bin/env bash
来源：http://hz.shzxlz.cn/gtgigohlrf.html

set -euo pipefail
来源：http://hz.0kj1m.cn/gtqnsnretp.html

[R02] 变量赋值与使用
来源：http://hz.haohaochexian.top/gtccskrqmx.html

name="Tom"; echo "$name"
来源：http://hz.zycfv.cn/gtvbrpgank.html

[R03] 只读变量
来源：http://hz.hongshengwenyu.top/gtbtjretjd.html

readonly PI=3.14
来源：http://hz.ppjwa.cn/gtrzpsayvi.html

[R04] 位置参数
来源：http://hz.wangdashe.top/gtkviigyxk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenlongwang.top/gtfskfpfwk.html

[R05] 参数默认值
来源：http://hz.quarkkingdee.top/gtihsuhbyk.html

name="${1:-default}"
来源：http://hz.yangfankeji.com/gtczceqydk.html

[R06] 判断命令是否存在
来源：http://hz.cashguo.top/gtfsqgmcku.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.mhx1999.top/gtgqnlxpid.html

[R07] if 判断文件
来源：http://hz.ybcxt.top/gtcnebbdwy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hywenlv.cn/gtkdenpbpj.html

[R08] 数值比较
来源：http://hz.aizwys.cn/gtjdscdfnb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yonumen.top/gtvasqzcdd.html

[R09] 字符串比较
来源：http://hz.zhijiandao.cn/gtxwndfcaj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ywan-chungtsiang.top/gtgwgjijqj.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtxapygwdm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yonumen.top/gtgvjfiouy.html

[R11] case 多分支
来源：http://hz.iojbl.cn/gtqybyhtau.html

case "$1" in
来源：http://hz.tian-w.cn/gtitgiabzo.html

start) echo "启动" ;;
来源：http://hz.gaohongyu789.top/gtdluxnwgl.html

stop)  echo "停止" ;;
来源：http://hz.smart0.xyz/gthtmgokci.html

*)     echo "未知命令" ;;
来源：http://hz.xziqi.cn/gtajpgoyhk.html

esac
来源：http://hz.yuxming.cn/gtezkenxbr.html

[R12] for 遍历文件
来源：http://hz.jianghu66.top/gtigirplok.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuxming.cn/gtnilvcdke.html

[R13] for 计数循环
来源：http://hz.jqgfzy.top/gtzmjfgznm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258.top/gtuigymvvb.html

[R14] C 风格 for
来源：http://hz.sweek.top/gtgaqhylze.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuanzx.com/gtjkribhjs.html

[R15] while 逐行读文件
来源：http://hz.hongshengwenyu.top/gtpkgkzigv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cucudq.cn/gtbiplznhg.html

[R16] until 等待条件
来源：http://hz.shangyingyoupin.top/gtoirtjvfm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gtndllsdmt.html

[R17] 数组定义与取值
来源：http://hz.hnqzz.top/gtmgcoqhaz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnqzz.top/gtnbadrfnt.html

[R18] 遍历数组
来源：http://hz.hysaishi.cn/gtcjtxigae.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ppjwa.cn/gtzywzbdeh.html

[R19] 数组长度
来源：http://hz.tianlin.xyz/gthzwagght.html

echo "${#arr[@]}"
来源：http://hz.svipenyu.cn/gtyabbwjaa.html

[R20] 关联数组（字典）
来源：http://hz.yanxiufei.cn/gttpekklka.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258.top/gtuiuzlotf.html

[R21] 字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtrqmckdnj.html

echo "${#s}"
来源：http://hz.yj20258.top/gtgbnrgdfe.html

[R22] 截取子串
来源：http://hz.tanke756.top/gtjooyroch.html

echo "${s:0:5}"
来源：http://hz.yuanzhike.top/gthjrrnnkj.html

[R23] 字符串替换
来源：http://hz.birdmap.top/gtijgorqlb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigfzy.top/gtntxzavxh.html

[R24] 大小写转换
来源：http://hz.ivvv.top/gtkozomvzl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fengsongda.top/gtrvvssdjh.html

[R25] 去后缀 / 去前缀
来源：http://hz.quarkkingdee.top/gtzetasvnw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aizwys.cn/gtdigefnej.html

[R26] 命令替换
来源：http://hz.pengpengdd.cyou/gtsejugqjc.html

now=$(date +%F); echo "$now"
来源：http://hz.yuanzhike.top/gtetwemgin.html

[R27] 算术展开
来源：http://hz.aibaodan.cn/gtrzwtnosb.html

echo $((1 + 2 * 3))
来源：http://hz.iojbl.cn/gtvdfqforu.html

[R28] 浮点运算
来源：http://hz.ydjk.org.cn/gtksipbclg.html

echo "scale=2; 10/3" | bc
来源：http://hz.wangdashe.top/gtweccudgm.html

[R29] 定义函数
来源：http://hz.nwbrower.top/gthyuhawcu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenjidiqi.icu/gtxetewltg.html

[R30] 函数返回状态码
来源：http://hz.nanxuanxn.top/gtuzbdadlk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yueranfly.top/gthtvrmxpm.html

[R31] 局部变量
来源：http://hz.0kj1m.cn/gtpiptziwp.html

f() { local x=1; echo "$x"; }
来源：http://hz.aibaodan.cn/gtfoodnxvu.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangtech.top/gtasuhcman.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtbmflkyts.html

[R33] 捕获错误并提示行号
来源：http://hz.jinyuanbaomall.cn/gthibrchnc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shuidangran.top/gtvwgjkpyo.html

[R34] 退出时清理
来源：http://hz.bjfxy.top/gtcjminefw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hongshengwenyu.top/gtypzgfbnh.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtptytdlyx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.daxiang520.top/gtsrievmuq.html

[R36] 并发执行多个任务
来源：http://hz.shzxlz.cn/gtyjhflbvy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnxiangtu.top/gtvafsppue.html

[R37] 把输出赋给变量
来源：http://hz.zdqjudy.top/gtfsjokjtq.html

files=$(ls -1)
来源：http://hz.gogol.net.cn/gtfkktsffh.html

[R38] 管道串联
来源：http://hz.tian-w.cn/gtbpkosxal.html

cat a.txt | grep -i error | wc -l
来源：http://hz.andypj.xyz/gtbnjhlsne.html

[R39] 重定向标准输出与错误
来源：http://hz.iojbl.cn/gtqshmdwuy.html

cmd > out.log 2>&1
来源：http://hz.yanxiufei.cn/gtvjizepag.html

[R40] 追加写日志
来源：http://hz.yueranfly.top/gtrbnswxge.html

echo "log" >> out.log
来源：http://hz.tian-w.cn/gttcagggar.html

[R41] 丢弃输出
来源：http://hz.hfpthk.cn/gtrlbhdnaf.html

cmd >/dev/null 2>&1
来源：http://hz.cashguo.top/gtcfyytiop.html

[R42] 输入重定向
来源：http://hz.chenjidiqi.icu/gtwmwpckqw.html

wc -l < a.txt
来源：http://hz.0kj1m.cn/gtlmraqpyo.html

[R43] 按名字查找文件
来源：http://hz.wangdashe.top/gtcmveaqii.html

find . -name "*.log" -type f
来源：http://hz.yongpay.top/gtxnjhfdkz.html

[R44] 按修改时间查找
来源：http://hz.sxryk.cn/gtdipraeze.html

find . -mtime -7 -type f
来源：http://hz.yanxiufei.cn/gtioougqql.html

[R45] 批量删除
来源：http://hz.c1oappe.top/gthpncuggu.html

find . -name "*.tmp" -delete
来源：http://hz.pycfn.com/gtezmsoyin.html

[R46] 递归替换文件内容
来源：http://hz.zhiwuduotai.top/gtoanhjqvr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sufxvd.cn/gtlniaijje.html

[R47] sed 单行替换
来源：http://hz.tianlin.xyz/gtaqgbhdso.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xinyue.icu/gtdmsgtyrk.html

[R48] awk 取指定列
来源：http://hz.zdqjudy.top/gtqpxghlrv.html

awk '{print $1, $3}' a.txt
来源：http://hz.jlsjyb.cn/gtzdbvdyrs.html

[R49] awk 带条件
来源：http://hz.zhongyouzk.top/gtzcccrody.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ehwqpu.com/gtdayhnopm.html

[R50] awk 求和
来源：http://hz.yonumen.top/gtwpkurahv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj202588.top/gtmzvrxwdk.html

[R51] 排序去重取前几
来源：http://hz.xuanzx.com/gtvxypiklq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258888.top/gtrgdfjeoj.html

[R52] 统计行数
来源：http://hz.xylfe.cn/gtxvibhszz.html

wc -l a.txt
来源：http://hz.zycfv.cn/gtwsbmentf.html

[R53] 查看文件头与实时尾
来源：http://hz.hfpthk.cn/gttlagukgx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jqgfzy.top/gtetphzivn.html

[R54] 比较两个文件
来源：http://hz.xingfuxueyuan.xyz/gtwajfkrtl.html

diff a.txt b.txt
来源：http://hz.yuanzhike.top/gtqftvqswr.html

[R55] 压缩与解压
来源：http://hz.0kj1m.cn/gtkffgtcii.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yonumen.top/gtpsovggmq.html

[R56] 远程拷贝
来源：http://hz.xziqi.cn/gtdpohrjjv.html

scp file user@host:/path/
来源：http://hz.ydzc1.top/gtvlcmeyja.html

[R57] 远程执行命令
来源：http://hz.zdqjudy.top/gtlzjbtcwp.html

ssh user@host 'uptime'
来源：http://hz.yj20258888.top/gtozrmjmtg.html

[R58] 下载文件
来源：http://hz.zhixingplan.top/gtqmmmpaev.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.andypj.xyz/gtgqanyqhe.html

[R59] 发 POST JSON
来源：http://hz.birdmap.top/gtbuxcgakl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.redwolf501.top/gtraviysjx.html

[R60] 只看 HTTP 状态码
来源：http://hz.gogol.net.cn/gtjgfrdidu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxuanxn.top/gtozrrfelq.html

[R61] 磁盘占用
来源：http://hz.yj20258.top/gtrsdasgnf.html

df -h;  du -sh *
来源：http://hz.ywan-chungtsiang.top/gtxhqtfssz.html

[R62] 找最占空间的文件
来源：http://hz.gogol.net.cn/gtzhanjewd.html

du -ah . | sort -rh | head -10
来源：http://hz.cqqwz.cn/gtwyoikaij.html

[R63] 内存与进程
来源：http://hz.yj20258.top/gtwvkcouvy.html

free -h;  ps aux | grep nginx
来源：http://hz.hfpthk.cn/gtkweatswg.html

[R64] 结束进程
来源：http://hz.zhengqikj.top/gtzfjnktxo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.dianchejie.cn/gtfyzzaltl.html

[R65] 查看端口占用
来源：http://hz.pycfn.com/gtbagunoos.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ybcxt.top/gtjfazvhxq.html

[R66] 定时任务
来源：http://hz.yuxming.cn/gtuoxrhjig.html

crontab -e;  crontab -l
来源：http://hz.fengsongda.top/gtdvdyrkdm.html

[R67] 生成随机十六进制串
来源：http://hz.fzhhl.top/gttpbrupsy.html

openssl rand -hex 16
来源：http://hz.yj20258.top/gtqwrvafle.html

[R68] 计算文件校验值
来源：http://hz.yanxiufei.cn/gtvjqehayu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tian-w.cn/gtflkxtjtn.html

[R69] 生成随机密码
来源：http://hz.zdqjudy.top/gtgufjdwji.html

head -c 16 /dev/urandom | base64
来源：http://hz.andypj.xyz/gtjgcmzydu.html

[R70] 时间戳与互转
来源：http://hz.xuetiantiany.cn/gtbdbtwaxz.html

date +%s;  date -d @1700000000
来源：http://hz.feifeiyinyue.top/gtxwabkzez.html

[R71] 日期格式化
来源：http://hz.dashuyun.cn/gteprpjzsd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tian-w.cn/gtgxywybxc.html

[R72] 等待端口就绪
来源：http://hz.nanxuanxn.top/gtcdkaoucd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhijiandao.cn/gtgfdwgekc.html

[R73] 分割大日志
来源：http://hz.yonumen.top/gtgohhjzfz.html

split -l 1000 big.log part_
来源：http://hz.havefunace.top/gtqaspusus.html

[R74] 批量重命名
来源：http://hz.zycfv.cn/gtezopbvfy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tianlin.xyz/gtcthkfdcl.html

[R75] 导出环境变量
来源：http://hz.cheryme.top/gtxmhoaoid.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtjjmfablp.html

[R76] 使用临时文件
来源：http://hz.chenjidiqi.icu/gtnvhbgqkp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.redwolf501.top/gtwqkuiwpy.html

[R77] 读取用户输入
来源：http://hz.chenlongwang.top/gthxwjpqwb.html

read -rp "请输入: " ans
来源：http://hz.xuetiantiany.cn/gtqmrpnqec.html

[R78] 交互式菜单
来源：http://hz.ydjk.org.cn/gteubvdtrz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxuanxn.top/gtwtdblgdv.html

[R79] 解析命令行选项
来源：http://hz.yuanzhike.top/gtfwlnddrd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhaomingkeji.xyz/gtdleacunk.html

[R80] 查看脚本执行耗时
来源：http://hz.gogol.net.cn/gtwzmdyoch.html

time ./run.sh
来源：http://hz.redwolf501.top/gtkalwsakx.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtdjutomne.html

S. C / C++ 专题
来源：http://hz.xinyue.icu/gtcqmfcils.html

================================================================================
来源：http://hz.ehwqpu.com/gtcszqrely.html

[S01] C：Hello World
来源：http://hz.jlsjyb.cn/gtjymxchnr.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gtgmtapxdb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daxiang520.top/gtoyetwrqa.html

[S02] C：变量与格式化输出
来源：http://hz.zdqjudy.top/gtxtaqjgxz.html

int a = 10; printf("%d\n", a);
来源：http://hz.c1oappe.top/gtzjwcqpsy.html

[S03] C：读入整数
来源：http://hz.zhixingplan.top/gtdfrgfxlk.html

int x; scanf("%d", &x);
来源：http://hz.yonumen.top/gteftixenz.html

[S04] C：字符串复制
来源：http://hz.ivvv.top/gtjsgctycl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xziqi.cn/gtkpkqpvyp.html

[S05] C：字符串长度
来源：http://hz.cucudq.cn/gtfrykvgmq.html

strlen(s)
来源：http://hz.daxiang520.top/gtshfbxynk.html

[S06] C：字符串比较
来源：http://hz.aibaodan.cn/gtwkhztlps.html

strcmp(a, b) == 0
来源：http://hz.xylfe.cn/gtqaalferj.html

[S07] C：数组遍历求和
来源：http://hz.birdmap.top/gtaduukdqv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dianchejie.cn/gtimybedsg.html

[S08] C：动态内存分配与释放
来源：http://hz.yongpay.top/gtqtwgfgse.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xuanzx.com/gttlgfvyco.html

[S09] C：结构体定义与初始化
来源：http://hz.zycfv.cn/gterrksqby.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yvedp.cn/gthqjoinrt.html

[S10] C：指针与解引用
来源：http://hz.jqgufenzy.top/gtvjftrnke.html

int *p = &a;  *p = 5;
来源：http://hz.birdmap.top/gtfoxhezcv.html

[S11] C：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtjyijsskf.html


<!-- 参考信息 -->