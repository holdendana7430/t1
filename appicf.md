代发 wailian999

[Q44] IN 子查询
来源：http://hz.gaohongyu789.top/gtngkpwwcn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenlongwang.top/gtpdojselo.html

[Q45] EXISTS 判断存在
来源：http://hz.xingfuxueyuan.xyz/gtrfahcluv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gtzyzuelwa.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.quarkkingdee.top/gtapvkrfxv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtesomwess.html

[Q47] 与平均值比较
来源：http://hz.gaohongyu789.top/gtjmsibigk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhixingplan.top/gtpmptdhlk.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtfdeivlbr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.redwolf501.top/gtasvbjvwi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hongshengwenyu.top/gtjeovjzlg.html

[Q49] 更新单行
来源：http://hz.svipenyu.cn/gtnulelpab.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dianchejie.cn/gtrpvnphfp.html

[Q50] 批量更新
来源：http://hz.ybcxt.top/gthlkmsqet.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinqigufen.top/gtqhbntetn.html

[Q51] 用子查询更新
来源：http://hz.wangshuangyany.cn/gtuvkyaotl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuanzhike.top/gtntbghhic.html

[Q52] 删除指定行
来源：http://hz.pengpengdd.cyou/gtbzimmcxj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtoezuncqf.html

[Q53] 按条件删除
来源：http://hz.ydjk.org.cn/gtxqrdpwyt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gzhubu.top/gtwmjvfkpp.html

[Q54] 清空表
来源：http://hz.pycfn.com/gthniotevj.html

TRUNCATE TABLE logs;
来源：http://hz.tianlin.xyz/gtgjapygka.html

[Q55] 排名（并列占位）
来源：http://hz.gaohongyu789.top/gtemjcmmxo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.feifeiyinyue.top/gtoohgislu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgfzy.top/gtakbrzuqo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gogol.net.cn/gtxthomxdd.html

[Q57] 行号
来源：http://hz.hysaishi.cn/gturtzfivu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuanzx.com/gttutzdtpt.html

[Q58] 累计求和
来源：http://hz.pycfn.com/gtifrugjni.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.andypj.xyz/gtpksizmwn.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtkmakdfsc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ybcxt.top/gthlfnebye.html

[Q60] 取上一行 / 下一行
来源：http://hz.yangfankeji.com/gtcfxvgwgo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cheryme.top/gtclfjdyjm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jyoumei.cn/gtrsefvgtw.html

[Q61] 移动平均
来源：http://hz.jinqigufen.top/gtkuhvnscd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xylfe.cn/gtmzggpfcx.html

[Q62] 分组占比
来源：http://hz.yangfankeji.com/gtzsutlsny.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sweek.top/gtvxgmtcpi.html

[Q63] 开启事务
来源：http://hz.mhx1999.top/gtvwdyqxbt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gaohongyu789.top/gtbjwvpihg.html

[Q64] 提交事务
来源：http://hz.shuidangran.top/gttwkjdlap.html

COMMIT;
来源：http://hz.nanxuanxn.top/gtdcgpaxiu.html

[Q65] 回滚事务
来源：http://hz.guowangkeji.top/gtipuftmgl.html

ROLLBACK;
来源：http://hz.sweek.top/gtaesrrmlf.html

[Q66] 行锁查询
来源：http://hz.yuanzhike.top/gtbjahxlqk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.bjfxy.top/gtucqunzwl.html

[Q67] 设置隔离级别
来源：http://hz.9152youxi.cn/gtftflajal.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jianghu66.top/gtarzfjovq.html

[Q68] 保存点
来源：http://hz.jinghuilouyu.cn/gthyinsbek.html

SAVEPOINT sp1;
来源：http://hz.bjfxy.top/gtalbabrou.html

ROLLBACK TO sp1;
来源：http://hz.hnqzz.top/gtfdkfbsrg.html

[Q69] 查看执行计划
来源：http://hz.guannengcc.top/gtfsxcxoph.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.mhx1999.top/gtzuzwxdnr.html

[Q70] 更新统计信息
来源：http://hz.fzhhl.top/gtceudyxvw.html

ANALYZE TABLE users;
来源：http://hz.guowangkeji.top/gtrxajxssy.html

[Q71] 查看建表语句
来源：http://hz.quarkkingdee.top/gtxprsifqw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pycfn.com/gtpgikgegj.html

[Q72] 查看索引
来源：http://hz.ywan-chungtsiang.top/gtzhojfeot.html

SHOW INDEX FROM users;
来源：http://hz.yj20258.top/gtsdtneasq.html

[Q73] 查看表状态
来源：http://hz.fengsongda.top/gtrseqsgwq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuanzhike.top/gtrjawqoyp.html

[Q74] 强制使用索引
来源：http://hz.52xcode.cn/gtvuczjgag.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nwbrower.top/gtfaibwcrw.html

[Q75] 日期格式化
来源：http://hz.hammf.cn/gtfcaoqqpd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xinyue.icu/gtmvwkbhgs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuxming.cn/gtyztqztnn.html

[Q76] 按天统计
来源：http://hz.zhengqikj.top/gtyrfvzjuh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.iojbl.cn/gtqyfdhczg.html

[Q77] 时间加减
来源：http://hz.gogol.net.cn/gtfqmkhrsp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yangfankeji.com/gtqxpeafgv.html

[Q78] 当前时间
来源：http://hz.cqqwz.cn/gtajbyxuht.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dashuyun.cn/gttfkwmgtt.html

[Q79] 字符串拼接
来源：http://hz.9152youxi.cn/gtjmqibvrr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.redwolf501.top/gttshbreip.html

[Q80] 字符串截取
来源：http://hz.nanxuanxn.top/gtrgfeeibg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangshuangyany.cn/gtjazqxaop.html

[Q81] 字符串替换
来源：http://hz.ivvv.top/gtcvmqhwwp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenlongwang.top/gtfyrakoxl.html

[Q82] 字符长度与字节长度
来源：http://hz.nwbrower.top/gttfdwqazc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtwcgxtzac.html

[Q83] 大小写转换
来源：http://hz.mhx1999.top/gtbxzrsame.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhixingplan.top/gtnqvohwwz.html

[Q84] 去除首尾空格
来源：http://hz.hysaishi.cn/gtlmzgufdp.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuanzhike.top/gtskvyzzmm.html

[Q85] 数值取整
来源：http://hz.shanyushiyangtech.top/gthvlyalrs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sufxvd.cn/gtrtjhnxil.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxuanxn.top/gtdxryjndf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xziqi.cn/gtksihugmk.html

[Q87] JSON 字段做条件
来源：http://hz.redwolf501.top/gtqizakohu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.smart0.xyz/gtckykiaiv.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangkeji.top/gtqhufftzg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.vqdsnc.cn/gtwmymdvvr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxuanxn.top/gtfcrfmosr.html

[Q89] 判断表是否存在
来源：http://hz.hnxiangtu.top/gtcnbyryua.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.iojbl.cn/gtrbjovrgm.html

[Q90] 生成序号列
来源：http://hz.yuanzhike.top/gtdqtumiam.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jiagoushi.top/gthbttgwbo.html

================================================================================
来源：http://hz.ivvv.top/gtuugzcanq.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtiejbcjie.html

================================================================================
来源：http://hz.sxryk.cn/gtiqqyjszj.html

[R01] shebang 与严格模式
来源：http://hz.ywan-chungtsiang.top/gtuximftwo.html

#!/usr/bin/env bash
来源：http://hz.shangyingyoupin.top/gtmvyevfyk.html

set -euo pipefail
来源：http://hz.haohaochexian.top/gtipbaeekc.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtajscadet.html

name="Tom"; echo "$name"
来源：http://hz.shzxlz.cn/gtdntxnhbl.html

[R03] 只读变量
来源：http://hz.ppjwa.cn/gtdymtemfc.html

readonly PI=3.14
来源：http://hz.sufxvd.cn/gtwxiihkgp.html

[R04] 位置参数
来源：http://hz.chenzaomai.com/gtmtwurvrx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinyuanbaomall.cn/gtwvwtvxbm.html

[R05] 参数默认值
来源：http://hz.jinyuanbaomall.cn/gtgaapilxm.html

name="${1:-default}"
来源：http://hz.jinyuanbaomall.cn/gtzhkfmnfd.html

[R06] 判断命令是否存在
来源：http://hz.fzhhl.top/gtcaeidbzx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sufxvd.cn/gtyqrjrsxd.html

[R07] if 判断文件
来源：http://hz.jinghuilouyu.cn/gtwylamesq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gtdleejwnw.html

[R08] 数值比较
来源：http://hz.jinyuanbaomall.cn/gtlaljyqlz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cucudq.cn/gtnjunqksr.html

[R09] 字符串比较
来源：http://hz.gotoacloud.top/gtzdyxdnik.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydzc1.top/gtmztpjfut.html

[R10] 正则匹配
来源：http://hz.shuidangran.top/gtqfnbynry.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgfzy.top/gtnwhhvntw.html

[R11] case 多分支
来源：http://hz.gzhubu.top/gtomgmzmuk.html

case "$1" in
来源：http://hz.hywenlv.cn/gtogfnztzx.html

start) echo "启动" ;;
来源：http://hz.feifeiyinyue.top/gtlniozyof.html

stop)  echo "停止" ;;
来源：http://hz.chenjidiqi.icu/gtlgnhswma.html

*)     echo "未知命令" ;;
来源：http://hz.smart0.xyz/gtgkcvkrti.html

esac
来源：http://hz.hywenlv.cn/gtigwrjdgb.html

[R12] for 遍历文件
来源：http://hz.wangdashe.top/gtmsdxfsxo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hysaishi.cn/gtmprugxze.html

[R13] for 计数循环
来源：http://hz.hongshengwenyu.top/gttxigkkrs.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.redwolf501.top/gtwzhhcbeh.html

[R14] C 风格 for
来源：http://hz.yonumen.top/gtdprypeet.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jianghu66.top/gtdyihdvsq.html

[R15] while 逐行读文件
来源：http://hz.sweek.top/gttljqtxdb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shzxlz.cn/gtfutdsbru.html

[R16] until 等待条件
来源：http://hz.yj202588.top/gtfmodhhsn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ehwqpu.com/gterodkdhl.html

[R17] 数组定义与取值
来源：http://hz.mhx1999.top/gttxpbnhlz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhengqikj.top/gtvttknwbe.html

[R18] 遍历数组
来源：http://hz.yueranfly.top/gtefnpyoae.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fengsongda.top/gtxsslnzhc.html

[R19] 数组长度
来源：http://hz.fzhhl.top/gtzfrwnwzr.html

echo "${#arr[@]}"
来源：http://hz.316326.xyz/gtrpslvrbb.html

[R20] 关联数组（字典）
来源：http://hz.9152youxi.cn/gtnuonoich.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.haohaochexian.top/gtjytmnspl.html

[R21] 字符串长度
来源：http://hz.gotoacloud.top/gtndcxcpic.html

echo "${#s}"
来源：http://hz.jinqigfzy.top/gtmhlcljop.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtoqcyrxly.html

echo "${s:0:5}"
来源：http://hz.jlsjyb.cn/gtcubqhdxb.html

[R23] 字符串替换
来源：http://hz.xuetiantiany.cn/gtbeexuyfl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.aibaodan.cn/gtdmtkgjew.html

[R24] 大小写转换
来源：http://hz.9152youxi.cn/gtyrygaaxx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenjidiqi.icu/gtfirsrmbv.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gtsxfedsdp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yanxiufei.cn/gtyqqfrhyl.html

[R26] 命令替换
来源：http://hz.yuxming.cn/gtvpkvadia.html

now=$(date +%F); echo "$now"
来源：http://hz.ivvv.top/gtntkktqnj.html

[R27] 算术展开
来源：http://hz.dashuyun.cn/gtfnndggrp.html

echo $((1 + 2 * 3))
来源：http://hz.chenzaomai.com/gtptxplfrd.html

[R28] 浮点运算
来源：http://hz.sysykeji.top/gtmagioilb.html

echo "scale=2; 10/3" | bc
来源：http://hz.cheryme.top/gtlgwqzbrm.html

[R29] 定义函数
来源：http://hz.9152youxi.cn/gttomqrxuy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gotoacloud.top/gtvywogajb.html

[R30] 函数返回状态码
来源：http://hz.andypj.xyz/gtwtkovoad.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258888.top/gtqggwdfip.html

[R31] 局部变量
来源：http://hz.ivvv.top/gtqdukanry.html

f() { local x=1; echo "$x"; }
来源：http://hz.9152youxi.cn/gthlfqtwhd.html

[R32] 参数个数校验
来源：http://hz.ybcxt.top/gtwkkasnci.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hnqzz.top/gtsfpbxffv.html

[R33] 捕获错误并提示行号
来源：http://hz.nanxuanxn.top/gthrgyxtpa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aibaodan.cn/gtcohcurpe.html

[R34] 退出时清理
来源：http://hz.guannengcc.top/gtocdfhuja.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtkmtxkder.html

[R35] 后台执行并等待
来源：http://hz.gaohongyu789.top/gtwamhpwbh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuanzx.com/gtutisbrto.html

[R36] 并发执行多个任务
来源：http://hz.mhx1999.top/gtiaujdlpq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj20258.top/gtpedrxrnz.html

[R37] 把输出赋给变量
来源：http://hz.316326.xyz/gtddipxtsk.html

files=$(ls -1)
来源：http://hz.jyoumei.cn/gtirhuwrew.html

[R38] 管道串联
来源：http://hz.zhongyouzk.top/gtqqmwijbo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dianchejie.cn/gtdfdqddyh.html

[R39] 重定向标准输出与错误
来源：http://hz.zycfv.cn/gtcwtdwjjg.html

cmd > out.log 2>&1
来源：http://hz.jinqigufen.top/gtsrftrfzj.html

[R40] 追加写日志
来源：http://hz.zhengqikj.top/gtlfexgsds.html

echo "log" >> out.log
来源：http://hz.zhijiandao.cn/gteyxbezla.html

[R41] 丢弃输出
来源：http://hz.cheryme.top/gtimqnlpme.html

cmd >/dev/null 2>&1
来源：http://hz.quarkkingdee.top/gtdmczjzla.html

[R42] 输入重定向
来源：http://hz.gotoacloud.top/gtqbumobew.html

wc -l < a.txt
来源：http://hz.ppjwa.cn/gttzghcobt.html

[R43] 按名字查找文件
来源：http://hz.zhaomingkeji.xyz/gtnzbpjayr.html

find . -name "*.log" -type f
来源：http://hz.yj20258888.top/gtwpznmyxf.html

[R44] 按修改时间查找
来源：http://hz.haohaochexian.top/gtwyjxiymx.html

find . -mtime -7 -type f
来源：http://hz.xinyue.icu/gtgqjfmxcj.html

[R45] 批量删除
来源：http://hz.zdqjudy.top/gtcrhbcpak.html

find . -name "*.tmp" -delete
来源：http://hz.chenzaomai.com/gtpvrlyomf.html

[R46] 递归替换文件内容
来源：http://hz.nanxuanxn.top/gtkcjckuqo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pycfn.com/gtjvoujiru.html

[R47] sed 单行替换
来源：http://hz.jiagoushi.top/gtfpmszaoj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinqigufen.top/gthhlsrije.html

[R48] awk 取指定列
来源：http://hz.gzhubu.top/gtbpdwwqtd.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuetiantiany.cn/gttywdpudf.html

[R49] awk 带条件
来源：http://hz.cucudq.cn/gtagqjdqou.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hnqzz.top/gtnagnmmxk.html

[R50] awk 求和
来源：http://hz.wangshuangyany.cn/gtmkyhtnap.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.kuanghao11.cn/gtxykjpity.html

[R51] 排序去重取前几
来源：http://hz.vqdsnc.cn/gtlrsgrqee.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aibaodan.cn/gtwrgybjce.html

[R52] 统计行数
来源：http://hz.cashguo.top/gtdlhusksu.html

wc -l a.txt
来源：http://hz.guannengcc.top/gtkfiolykk.html

[R53] 查看文件头与实时尾
来源：http://hz.zhengqikj.top/gtmmzliaqr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hfpthk.cn/gtgppojbcy.html

[R54] 比较两个文件
来源：http://hz.sweek.top/gttwhquqrp.html

diff a.txt b.txt
来源：http://hz.yj20258888.top/gtykzxisud.html

[R55] 压缩与解压
来源：http://hz.daria6918.cn/gtyiizawrs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.meibo888.top/gtcblmrmqj.html

[R56] 远程拷贝
来源：http://hz.tian-w.cn/gtsxariuno.html

scp file user@host:/path/
来源：http://hz.xingfuxueyuan.xyz/gtmvexzrmb.html

[R57] 远程执行命令
来源：http://hz.316326.xyz/gtxpruyctx.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangkeji.top/gtjjoxsqdb.html

[R58] 下载文件
来源：http://hz.hnxiangtu.top/gtdptaemer.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gaohongyu789.top/gtjzdnffdx.html

[R59] 发 POST JSON
来源：http://hz.xingfuxueyuan.xyz/gtvtrddztn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangtech.top/gtevytdgse.html

[R60] 只看 HTTP 状态码
来源：http://hz.tian-w.cn/gtfflvorfv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhaomingkeji.xyz/gtdykupsos.html

[R61] 磁盘占用
来源：http://hz.yanxiufei.cn/gtxdkhcyfo.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtdlbzansi.html

[R62] 找最占空间的文件
来源：http://hz.xylfe.cn/gtbczfsgme.html

du -ah . | sort -rh | head -10
来源：http://hz.ehwqpu.com/gtqrshoade.html

[R63] 内存与进程
来源：http://hz.yj20258888.top/gtfeahdkrv.html

free -h;  ps aux | grep nginx
来源：http://hz.gzhubu.top/gthckbrkxn.html

[R64] 结束进程
来源：http://hz.yangfankeji.com/gtsibehrmy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgfzy.top/gtxujhnqef.html

[R65] 查看端口占用
来源：http://hz.birdmap.top/gtaiiqbkmj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fzhhl.top/gtfeakojii.html

[R66] 定时任务
来源：http://hz.tanke756.top/gtujrucznt.html

crontab -e;  crontab -l
来源：http://hz.xinyue.icu/gthbbpewjd.html

[R67] 生成随机十六进制串
来源：http://hz.tianlin.xyz/gtmybiusmt.html

openssl rand -hex 16
来源：http://hz.snrcjt.cn/gttgeqnjwi.html

[R68] 计算文件校验值
来源：http://hz.gaohongyu789.top/gtmgjdjpjb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cqqwz.cn/gtkqqeglqt.html

[R69] 生成随机密码
来源：http://hz.yueranfly.top/gtxltnjpey.html

head -c 16 /dev/urandom | base64
来源：http://hz.fengsongda.top/gtpstcocjg.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtykmntzfp.html

date +%s;  date -d @1700000000
来源：http://hz.hongshengwenyu.top/gtuveqlnrf.html

[R71] 日期格式化
来源：http://hz.316326.xyz/gtdshxitst.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yongpay.top/gtvqqwbftu.html

[R72] 等待端口就绪
来源：http://hz.yongpay.top/gttrwbjoxd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ybcxt.top/gtycasqxql.html

[R73] 分割大日志
来源：http://hz.smart0.xyz/gtbvegqett.html

split -l 1000 big.log part_
来源：http://hz.cucudq.cn/gthecppciw.html

[R74] 批量重命名
来源：http://hz.52xcode.cn/gtaudacvzx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pengpengdd.cyou/gtmkzrsxbp.html

[R75] 导出环境变量
来源：http://hz.ivvv.top/gtmbjnyhdo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gtweexedaf.html

[R76] 使用临时文件
来源：http://hz.hfpthk.cn/gtezcnrnob.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtbuglfktk.html

[R77] 读取用户输入
来源：http://hz.ydjk.org.cn/gtkvfjkwxh.html

read -rp "请输入: " ans
来源：http://hz.daxiang520.top/gttbvzmecb.html

[R78] 交互式菜单
来源：http://hz.cdnleiting.top/gtrejcsaai.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tanke756.top/gtgamfbvba.html

[R79] 解析命令行选项
来源：http://hz.jinghuilouyu.cn/gtkjzmdezh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daxiang520.top/gtdmwugaxg.html

[R80] 查看脚本执行耗时
来源：http://hz.tanke756.top/gtxslaspdo.html

time ./run.sh
来源：http://hz.cheryme.top/gtmcackktz.html

================================================================================
来源：http://hz.gotoacloud.top/gttksjozkz.html

S. C / C++ 专题
来源：http://hz.yj20258888.top/gtnkfikxvn.html

================================================================================
来源：http://hz.svipenyu.cn/gtfgxedpdh.html

[S01] C：Hello World
来源：http://hz.andypj.xyz/gtijxwhphu.html

#include <stdio.h>
来源：http://hz.nwbrower.top/gtmekpikqe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yongpay.top/gtjwabtcri.html

[S02] C：变量与格式化输出
来源：http://hz.zhongyouzk.top/gtcqcjjpjt.html

int a = 10; printf("%d\n", a);
来源：http://hz.gotoacloud.top/gtefmbrtfh.html

[S03] C：读入整数
来源：http://hz.hnqzz.top/gtuaeefrlu.html

int x; scanf("%d", &x);
来源：http://hz.yuanzhike.top/gtjciwuqry.html

[S04] C：字符串复制
来源：http://hz.zhixingplan.top/gtaicvjitt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtdjbccsak.html

[S05] C：字符串长度
来源：http://hz.yvedp.cn/gtajozjtdb.html

strlen(s)
来源：http://hz.jinyuanbaomall.cn/gtdghdccnl.html

[S06] C：字符串比较
来源：http://hz.nanxinkj.top/gtsznenafc.html

strcmp(a, b) == 0
来源：http://hz.shangyingyoupin.top/gtwmsxugkd.html

[S07] C：数组遍历求和
来源：http://hz.chenzaomai.com/gtpoauqoka.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yanxiufei.cn/gtdydegcda.html

[S08] C：动态内存分配与释放
来源：http://hz.mhx1999.top/gtynuepizu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgufenzy.top/gthxpfwmue.html

[S09] C：结构体定义与初始化
来源：http://hz.ppjwa.cn/gtcyjgrojv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258888.top/gtekwozqtm.html

[S10] C：指针与解引用
来源：http://hz.jiagoushi.top/gtfggalfte.html

int *p = &a;  *p = 5;
来源：http://hz.aibaodan.cn/gtmghonhur.html

[S11] C：逐行读文件
来源：http://hz.zhongyouzk.top/gtdinpsimz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pengpengdd.cyou/gtiovbtsid.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cqqwz.cn/gtfgumhnie.html

fclose(f);
来源：http://hz.zhongyouzk.top/gtkadurqsw.html

[S12] C：写文件
来源：http://hz.snrcjt.cn/gtzivlgogy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.c1oappe.top/gtootyyfqg.html

[S13] C：宏定义
来源：http://hz.ehwqpu.com/gtfrthrzyj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtzftgkzgf.html

[S14] C：枚举
来源：http://hz.sufxvd.cn/gtaxbwltkz.html


<!-- 参考信息 -->