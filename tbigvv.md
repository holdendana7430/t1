代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aibaodan.cn/gtjgbhqbir.html

[Q58] 累计求和
来源：http://hz.zhoulong.xyz/gtbxbvbacj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxuanxn.top/gtkgjxjmml.html

[Q59] 分组内累计
来源：http://hz.bjfxy.top/gtmfitnwsa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cqqwz.cn/gtefavsnrp.html

[Q60] 取上一行 / 下一行
来源：http://hz.hongshengwenyu.top/gtqqkshstu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shangyingyoupin.top/gtkkpqtpgl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gtsefyalur.html

[Q61] 移动平均
来源：http://hz.shanyushiyangtech.top/gtgfrqptnn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hysaishi.cn/gtsbntfewa.html

[Q62] 分组占比
来源：http://hz.yongpay.top/gtuudhytor.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gticzypxqt.html

[Q63] 开启事务
来源：http://hz.pycfn.com/gttxxxdesz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yanxiufei.cn/gtpwwapojc.html

[Q64] 提交事务
来源：http://hz.quarkkingdee.top/gtaeexvkvp.html

COMMIT;
来源：http://hz.aizwys.cn/gtkserteko.html

[Q65] 回滚事务
来源：http://hz.xylfe.cn/gtlfxkywwk.html

ROLLBACK;
来源：http://hz.wangdashe.top/gtlvuljhvp.html

[Q66] 行锁查询
来源：http://hz.nanxuanxn.top/gtwzwgxont.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yangfankeji.com/gtmrqttwqt.html

[Q67] 设置隔离级别
来源：http://hz.hywenlv.cn/gtgfcfdyqq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dashuyun.cn/gttqfbdepp.html

[Q68] 保存点
来源：http://hz.xinyue.icu/gtbxcsspiy.html

SAVEPOINT sp1;
来源：http://hz.pengpengdd.cyou/gtwzorxylt.html

ROLLBACK TO sp1;
来源：http://hz.zhiwuduotai.top/gtrjrkgvmu.html

[Q69] 查看执行计划
来源：http://hz.andypj.xyz/gtdzezfurf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yanxiufei.cn/gthjltutyx.html

[Q70] 更新统计信息
来源：http://hz.haohaochexian.top/gthumikhwq.html

ANALYZE TABLE users;
来源：http://hz.kuanghao11.cn/gttvjgsiky.html

[Q71] 查看建表语句
来源：http://hz.andypj.xyz/gtetcigtsn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.316326.xyz/gtlusgdioa.html

[Q72] 查看索引
来源：http://hz.sysykeji.top/gtnktjbhrb.html

SHOW INDEX FROM users;
来源：http://hz.c1oappe.top/gtvonhdgsd.html

[Q73] 查看表状态
来源：http://hz.hammf.cn/gtcgnvihwn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shuidangran.top/gtwcnnzxpm.html

[Q74] 强制使用索引
来源：http://hz.snrcjt.cn/gtzlluwsgi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xinyue.icu/gtbuixopdo.html

[Q75] 日期格式化
来源：http://hz.yanxiufei.cn/gtzvgucnmm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gtbwcwxbyc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.316326.xyz/gttaudrjlm.html

[Q76] 按天统计
来源：http://hz.yongpay.top/gtmvnjpudq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydzc1.top/gtuogbedxk.html

[Q77] 时间加减
来源：http://hz.ivvv.top/gttlegfhlp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xuanzx.com/gtsvigsycp.html

[Q78] 当前时间
来源：http://hz.pengpengdd.cyou/gtwpxddgox.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ppjwa.cn/gtwsjhjyja.html

[Q79] 字符串拼接
来源：http://hz.dashuyun.cn/gtcbaxocyi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cucudq.cn/gtoylgwmmi.html

[Q80] 字符串截取
来源：http://hz.nanxinkj.top/gtsgtiocca.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aibaodan.cn/gtxtyxpgib.html

[Q81] 字符串替换
来源：http://hz.chenjidiqi.icu/gtfocwguph.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yueranfly.top/gtezuselfr.html

[Q82] 字符长度与字节长度
来源：http://hz.jqgufenzy.top/gtokmmxhia.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tanke756.top/gtzpexbuqf.html

[Q83] 大小写转换
来源：http://hz.ydzc1.top/gtavwvgvxj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhijiandao.cn/gtwtysjbqx.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtkusohran.html

SELECT TRIM(name) FROM users;
来源：http://hz.vqdsnc.cn/gtvsnersrw.html

[Q85] 数值取整
来源：http://hz.wangdashe.top/gtnazlalqa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgufenzy.top/gtsjgwevow.html

[Q86] 读取 JSON 字段
来源：http://hz.cdnleiting.top/gtbcktbtvr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jyoumei.cn/gtpeiravkk.html

[Q87] JSON 字段做条件
来源：http://hz.guannengcc.top/gtzcishjdk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.mhx1999.top/gthudqevjv.html

[Q88] 行转列（条件聚合）
来源：http://hz.sweek.top/gtpvtmwxtf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.andypj.xyz/gtkxrcdqcq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtrlxcpbvx.html

[Q89] 判断表是否存在
来源：http://hz.kuanghao11.cn/gtkljybzrp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sufxvd.cn/gttebiqxhq.html

[Q90] 生成序号列
来源：http://hz.hnxiangtu.top/gtljszjehw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.smart0.xyz/gthrttfgme.html

================================================================================
来源：http://hz.cucudq.cn/gtvafmunef.html

R. Bash 专题
来源：http://hz.chenzaomai.com/gthmmkjvka.html

================================================================================
来源：http://hz.cdnleiting.top/gtfezouqzr.html

[R01] shebang 与严格模式
来源：http://hz.quarkkingdee.top/gtrbvfmjjp.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtrmagriil.html

set -euo pipefail
来源：http://hz.ivvv.top/gtipdhtggp.html

[R02] 变量赋值与使用
来源：http://hz.xziqi.cn/gtuxhhmoem.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gtqikvecad.html

[R03] 只读变量
来源：http://hz.birdmap.top/gtjpnvdbni.html

readonly PI=3.14
来源：http://hz.quarkkingdee.top/gtbadjttpf.html

[R04] 位置参数
来源：http://hz.yj20258.top/gtvvkrqejd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gtkhfoxghc.html

[R05] 参数默认值
来源：http://hz.wangshuangyany.cn/gtpdaztzkz.html

name="${1:-default}"
来源：http://hz.xziqi.cn/gtncewcder.html

[R06] 判断命令是否存在
来源：http://hz.jyoumei.cn/gtpfwhmmir.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtjeghgxmc.html

[R07] if 判断文件
来源：http://hz.hongshengwenyu.top/gtfihtcgxq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.smart0.xyz/gtcvbegofy.html

[R08] 数值比较
来源：http://hz.jlsjyb.cn/gtorucwplr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pycfn.com/gtbhjlcahz.html

[R09] 字符串比较
来源：http://hz.haohaochexian.top/gtwrbtujkp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ehwqpu.com/gtbhqerluj.html

[R10] 正则匹配
来源：http://hz.aibaodan.cn/gttayqoull.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sweek.top/gtdzxdflwb.html

[R11] case 多分支
来源：http://hz.dashuyun.cn/gtliqkytwa.html

case "$1" in
来源：http://hz.hongshengwenyu.top/gtbsvclxny.html

start) echo "启动" ;;
来源：http://hz.tian-w.cn/gtefzsecej.html

stop)  echo "停止" ;;
来源：http://hz.havefunace.top/gtpqmonnjr.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigfzy.top/gtmepfcfds.html

esac
来源：http://hz.yueranfly.top/gtnefkdiho.html

[R12] for 遍历文件
来源：http://hz.birdmap.top/gtcpdfcdtj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.mhx1999.top/gthvcyefgu.html

[R13] for 计数循环
来源：http://hz.yuanzhike.top/gtxjfgraol.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.havefunace.top/gtmzyocxuy.html

[R14] C 风格 for
来源：http://hz.aizwys.cn/gtzycvpaxm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hysaishi.cn/gtyeutyxxt.html

[R15] while 逐行读文件
来源：http://hz.hnxiangtu.top/gtrsdmvlhk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sxryk.cn/gtbbgnmwff.html

[R16] until 等待条件
来源：http://hz.cucudq.cn/gtuimcijvs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gzhubu.top/gtvhbhabti.html

[R17] 数组定义与取值
来源：http://hz.ivvv.top/gtdjsfnvfb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nwbrower.top/gtkgvycmin.html

[R18] 遍历数组
来源：http://hz.xingfuxueyuan.xyz/gtpzqkpwhw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cucudq.cn/gtfoftuqez.html

[R19] 数组长度
来源：http://hz.jinqigufen.top/gtdaxluvfs.html

echo "${#arr[@]}"
来源：http://hz.hammf.cn/gttcpmymuj.html

[R20] 关联数组（字典）
来源：http://hz.tianlin.xyz/gtgbtftvop.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnxiangtu.top/gtnjnrckzg.html

[R21] 字符串长度
来源：http://hz.shzxlz.cn/gttpaetqly.html

echo "${#s}"
来源：http://hz.andypj.xyz/gtzpguzeyo.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtffppyjtq.html

echo "${s:0:5}"
来源：http://hz.smart0.xyz/gtknmpiqkv.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gtyzlqhacf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.guowangkeji.top/gtlacpecie.html

[R24] 大小写转换
来源：http://hz.ivvv.top/gtjssakdqz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydzc1.top/gtvvphstks.html

[R25] 去后缀 / 去前缀
来源：http://hz.daria6918.cn/gtfbsxynby.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenjidiqi.icu/gtkpicvdws.html

[R26] 命令替换
来源：http://hz.gotoacloud.top/gtbevwzpik.html

now=$(date +%F); echo "$now"
来源：http://hz.xuetiantiany.cn/gthlzaqsnt.html

[R27] 算术展开
来源：http://hz.yangfankeji.com/gtgdyocidf.html

echo $((1 + 2 * 3))
来源：http://hz.meibo888.top/gtnarkhpsa.html

[R28] 浮点运算
来源：http://hz.zhijiandao.cn/gtdjxrkkaq.html

echo "scale=2; 10/3" | bc
来源：http://hz.haohaochexian.top/gtlonoboxr.html

[R29] 定义函数
来源：http://hz.vqdsnc.cn/gtcixotbyc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yanxiufei.cn/gtnajklgfw.html

[R30] 函数返回状态码
来源：http://hz.birdmap.top/gtuhrltqut.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgfzy.top/gtrascyzbx.html

[R31] 局部变量
来源：http://hz.nanxinkj.top/gtltmpbtrj.html

f() { local x=1; echo "$x"; }
来源：http://hz.ybcxt.top/gtwuenqiss.html

[R32] 参数个数校验
来源：http://hz.9152youxi.cn/gtpcaycyie.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.0kj1m.cn/gthsbcnvpn.html

[R33] 捕获错误并提示行号
来源：http://hz.birdmap.top/gtajgvhzcz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydjk.org.cn/gtfasrhmcm.html

[R34] 退出时清理
来源：http://hz.ydjk.org.cn/gtthntxrzs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtgoryixsf.html

[R35] 后台执行并等待
来源：http://hz.jinyuanbaomall.cn/gtltqvjren.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.mhx1999.top/gtakibwjoq.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtrobxxnpo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yonumen.top/gttyelvahn.html

[R37] 把输出赋给变量
来源：http://hz.gzhubu.top/gtmawlsspv.html

files=$(ls -1)
来源：http://hz.52xcode.cn/gtvmwvqgss.html

[R38] 管道串联
来源：http://hz.cqqwz.cn/gtwzidodbx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtrtwbullg.html

[R39] 重定向标准输出与错误
来源：http://hz.yonumen.top/gtzrbqwsqd.html

cmd > out.log 2>&1
来源：http://hz.chenzaomai.com/gtorvgfnun.html

[R40] 追加写日志
来源：http://hz.52xcode.cn/gtwplilkhw.html

echo "log" >> out.log
来源：http://hz.xziqi.cn/gttcxjoktf.html

[R41] 丢弃输出
来源：http://hz.nwbrower.top/gtkgpvmfli.html

cmd >/dev/null 2>&1
来源：http://hz.daria6918.cn/gtuovazgce.html

[R42] 输入重定向
来源：http://hz.birdmap.top/gtjfyaohmg.html

wc -l < a.txt
来源：http://hz.jiagoushi.top/gtgdqyjexs.html

[R43] 按名字查找文件
来源：http://hz.haohaochexian.top/gtyivkouky.html

find . -name "*.log" -type f
来源：http://hz.yj202588.top/gtlbplrlyx.html

[R44] 按修改时间查找
来源：http://hz.yj202588.top/gtxmdliheu.html

find . -mtime -7 -type f
来源：http://hz.sweek.top/gtawojzraz.html

[R45] 批量删除
来源：http://hz.jlsjyb.cn/gtinzzhqss.html

find . -name "*.tmp" -delete
来源：http://hz.ivvv.top/gtqnqqvwpl.html

[R46] 递归替换文件内容
来源：http://hz.jinqigfzy.top/gtmbkvxshn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jiagoushi.top/gtkvomicsg.html

[R47] sed 单行替换
来源：http://hz.0kj1m.cn/gthoenkglm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258.top/gtpjtcvtvt.html

[R48] awk 取指定列
来源：http://hz.tianlin.xyz/gtcnvtmsdi.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhengqikj.top/gtxvssnldi.html

[R49] awk 带条件
来源：http://hz.jinyuanbaomall.cn/gtiqzzdnml.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jiagoushi.top/gtfclrzqhe.html

[R50] awk 求和
来源：http://hz.yj202588.top/gtlqgthiva.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shzxlz.cn/gtvygiommw.html

[R51] 排序去重取前几
来源：http://hz.zhengqikj.top/gtszweqjku.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258.top/gtbdxgpwgi.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gttjlyoqmn.html

wc -l a.txt
来源：http://hz.yvedp.cn/gtazmmnwpl.html

[R53] 查看文件头与实时尾
来源：http://hz.cashguo.top/gtcvkrumpc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxuanxn.top/gtpmnoizih.html

[R54] 比较两个文件
来源：http://hz.chenjidiqi.icu/gtrilaxmcz.html

diff a.txt b.txt
来源：http://hz.vqdsnc.cn/gtclhxocbc.html

[R55] 压缩与解压
来源：http://hz.hnxiangtu.top/gtjqlrzimu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj202588.top/gtgcxiwujn.html

[R56] 远程拷贝
来源：http://hz.xylfe.cn/gtmadttxmv.html

scp file user@host:/path/
来源：http://hz.yangfankeji.com/gtdtfeodgn.html

[R57] 远程执行命令
来源：http://hz.yangfankeji.com/gthmorgyqw.html

ssh user@host 'uptime'
来源：http://hz.smart0.xyz/gtnfbrbmdq.html

[R58] 下载文件
来源：http://hz.snrcjt.cn/gtvxsptbdu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gotoacloud.top/gtjzlrnusf.html

[R59] 发 POST JSON
来源：http://hz.xuanzx.com/gtjdngtbia.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj202588.top/gtyrfyeyzo.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhengqikj.top/gtnndcajyv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gthbtvdquq.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangkeji.top/gtxuqivhpa.html

df -h;  du -sh *
来源：http://hz.yuxming.cn/gtgjpzzvhg.html

[R62] 找最占空间的文件
来源：http://hz.kuanghao11.cn/gtnpcspghk.html

du -ah . | sort -rh | head -10
来源：http://hz.zdqjudy.top/gtezqtpuck.html

[R63] 内存与进程
来源：http://hz.yonumen.top/gtqbqucnvy.html

free -h;  ps aux | grep nginx
来源：http://hz.cucudq.cn/gtxaydrjde.html

[R64] 结束进程
来源：http://hz.yangfankeji.com/gtwgznijmq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.316326.xyz/gteeqvuhbh.html

[R65] 查看端口占用
来源：http://hz.xuetiantiany.cn/gtomjomfcx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.snrcjt.cn/gtrghjhhit.html

[R66] 定时任务
来源：http://hz.zhijiandao.cn/gtzssgfigq.html

crontab -e;  crontab -l
来源：http://hz.jyoumei.cn/gtgxdwhpmn.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtxsbtxlkr.html

openssl rand -hex 16
来源：http://hz.smart0.xyz/gtfyriqsya.html

[R68] 计算文件校验值
来源：http://hz.yangfankeji.com/gtiszmuysb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cqqwz.cn/gtcnqbpmwb.html

[R69] 生成随机密码
来源：http://hz.jlsjyb.cn/gtlsntnmap.html

head -c 16 /dev/urandom | base64
来源：http://hz.yangfankeji.com/gtcqlvnmyx.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtipbbzhtn.html

date +%s;  date -d @1700000000
来源：http://hz.xuanzx.com/gtqainzuup.html

[R71] 日期格式化
来源：http://hz.nanxinkj.top/gtrqhvonjg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.316326.xyz/gtizrzunig.html

[R72] 等待端口就绪
来源：http://hz.tanke756.top/gtuisgzyow.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtrichrdgu.html

[R73] 分割大日志
来源：http://hz.jyoumei.cn/gtxaojczrq.html

split -l 1000 big.log part_
来源：http://hz.redwolf501.top/gtievkpzfz.html

[R74] 批量重命名
来源：http://hz.sufxvd.cn/gtlqnfsymt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jiagoushi.top/gtsyrxckkg.html

[R75] 导出环境变量
来源：http://hz.yuanzhike.top/gtuginzacj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tanke756.top/gteqxpiicx.html

[R76] 使用临时文件
来源：http://hz.yangfankeji.com/gtwsbqxjgz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guannengcc.top/gtfvbsgcmf.html

[R77] 读取用户输入
来源：http://hz.jqgufenzy.top/gtdnqqubdx.html

read -rp "请输入: " ans
来源：http://hz.jianghu66.top/gtcnveshej.html

[R78] 交互式菜单
来源：http://hz.chenjidiqi.icu/gtnfeoltkh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jianghu66.top/gtbxldpszb.html

[R79] 解析命令行选项
来源：http://hz.hammf.cn/gtixnlvfxr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sysykeji.top/gtspdibztq.html

[R80] 查看脚本执行耗时
来源：http://hz.zhiwuduotai.top/gtnmcquhqe.html

time ./run.sh
来源：http://hz.jinqigufen.top/gthdyebgsp.html

================================================================================
来源：http://hz.xziqi.cn/gtbslqdegc.html

S. C / C++ 专题
来源：http://hz.feifeiyinyue.top/gtaomfcgow.html

================================================================================
来源：http://hz.316326.xyz/gtowpajxdx.html

[S01] C：Hello World
来源：http://hz.gaohongyu789.top/gtmbswjbgx.html

#include <stdio.h>
来源：http://hz.ywan-chungtsiang.top/gtnzyclxoz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuxming.cn/gtsnlewpxh.html

[S02] C：变量与格式化输出
来源：http://hz.tianlin.xyz/gthbylalih.html

int a = 10; printf("%d\n", a);
来源：http://hz.havefunace.top/gtxcgaqjjp.html

[S03] C：读入整数
来源：http://hz.xuetiantiany.cn/gtnmeypfdc.html

int x; scanf("%d", &x);
来源：http://hz.nanxinkj.top/gtmjxujjkg.html

[S04] C：字符串复制
来源：http://hz.cheryme.top/gtobnqwqgs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jyoumei.cn/gtbiuhgugz.html

[S05] C：字符串长度
来源：http://hz.ybcxt.top/gtdvhzgthm.html

strlen(s)
来源：http://hz.aibaodan.cn/gtdfohstdw.html

[S06] C：字符串比较
来源：http://hz.yanxiufei.cn/gtmksfezhe.html

strcmp(a, b) == 0
来源：http://hz.tanke756.top/gtxonzpakg.html

[S07] C：数组遍历求和
来源：http://hz.nanxinkj.top/gtdoqkmgeg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydjk.org.cn/gtmyppicjn.html

[S08] C：动态内存分配与释放
来源：http://hz.wangdashe.top/gtukupdqaw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.dashuyun.cn/gtbxwmrlkl.html

[S09] C：结构体定义与初始化
来源：http://hz.haohaochexian.top/gtqtxgjotc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydjk.org.cn/gtorgnfpkc.html

[S10] C：指针与解引用
来源：http://hz.aibaodan.cn/gtechxbejh.html

int *p = &a;  *p = 5;
来源：http://hz.ppjwa.cn/gtilruspkk.html

[S11] C：逐行读文件
来源：http://hz.jyoumei.cn/gtrtmjjvpq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ywan-chungtsiang.top/gtyamafnvf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shuidangran.top/gtuinbkofh.html

fclose(f);
来源：http://hz.wangshuangyany.cn/gtlyfciobl.html

[S12] C：写文件
来源：http://hz.dashuyun.cn/gthxbqpsxo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pycfn.com/gtuealhvxf.html

[S13] C：宏定义
来源：http://hz.yonumen.top/gtkcowbxnc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pengpengdd.cyou/gtrnfqtuwp.html

[S14] C：枚举
来源：http://hz.yuanzhike.top/gtbgxdcosl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgfzy.top/gtfmzbfyvq.html

[S15] C：类型转换
来源：http://hz.hnxiangtu.top/gtikmfmomc.html

(double) a / b
来源：http://hz.sysykeji.top/gtxnnqphpb.html

[S16] C：位操作置位
来源：http://hz.9152youxi.cn/gtywoqshcp.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtbnopmaee.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtsibpbkvf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cucudq.cn/gtstxcguuh.html

[S18] C：命令行参数
来源：http://hz.yueranfly.top/gtqhcafhvn.html

int main(int argc, char **argv)
来源：http://hz.quarkkingdee.top/gtztcvjyyz.html

[S19] C：快速排序
来源：http://hz.zhengqikj.top/gtmfitcecf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gzhubu.top/gthvgdzpnu.html

[S20] C：二分查找
来源：http://hz.nwbrower.top/gtklorchzp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtjocfcttw.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gtcolakfzl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sufxvd.cn/gtcsocmeha.html

[S22] C：字符串转数字
来源：http://hz.shuidangran.top/gtkszphnoy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenzaomai.com/gtofjudtli.html

[S23] C：随机数
来源：http://hz.ehwqpu.com/gtuewkmbgg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuanzx.com/gtqoilnpvc.html

[S24] C：获取本地时间
来源：http://hz.gotoacloud.top/gtzylvghkq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zycfv.cn/gtlsvceica.html

[S25] C：内存拷贝
来源：http://hz.ydjk.org.cn/gtntakjxli.html

memcpy(dst, src, n);
来源：http://hz.shanyushiyangtech.top/gtikcbkssd.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gtfspxnwrp.html

memset(a, 0, sizeof a);
来源：http://hz.hongshengwenyu.top/gttjbnmmai.html

[S27] C：定义常量
来源：http://hz.9152youxi.cn/gttwvxttko.html

const double PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtrpkmfpzk.html

[S28] C：静态变量
来源：http://hz.dashuyun.cn/gtipwwygcm.html


<!-- 参考信息 -->