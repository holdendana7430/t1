代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.dashuyun.cn/gtttcafdsn.html

[Q58] 累计求和
来源：http://hz.guowangkeji.top/gtpcjbfsba.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ivvv.top/gtswwmoahr.html

[Q59] 分组内累计
来源：http://hz.hnxiangtu.top/gtnkuylfkf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.haohaochexian.top/gttlttolku.html

[Q60] 取上一行 / 下一行
来源：http://hz.kuanghao11.cn/gtwnxgmcnt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tanke756.top/gtabxuckuu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jlsjyb.cn/gtrjvnrooe.html

[Q61] 移动平均
来源：http://hz.yuxming.cn/gtjmxflaxw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xuanzx.com/gtmphwjlgw.html

[Q62] 分组占比
来源：http://hz.shanyushiyangtech.top/gttnypjmmm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtlaclxweo.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtetnyezfp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtentmxugo.html

[Q64] 提交事务
来源：http://hz.fzhhl.top/gtwudwglny.html

COMMIT;
来源：http://hz.ydzc1.top/gtwexddufp.html

[Q65] 回滚事务
来源：http://hz.gaohongyu789.top/gtmoivpvag.html

ROLLBACK;
来源：http://hz.hammf.cn/gtcioweplw.html

[Q66] 行锁查询
来源：http://hz.gaohongyu789.top/gtahcmtavs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.birdmap.top/gtubyseaof.html

[Q67] 设置隔离级别
来源：http://hz.cdnleiting.top/gtoxpstebn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gtttvvgtqq.html

[Q68] 保存点
来源：http://hz.jinghuilouyu.cn/gtmrebrrkc.html

SAVEPOINT sp1;
来源：http://hz.nanxuanxn.top/gtiwjzdzfs.html

ROLLBACK TO sp1;
来源：http://hz.hnxiangtu.top/gtlmqknyew.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gtdldsokfa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hnxiangtu.top/gtylmvsawl.html

[Q70] 更新统计信息
来源：http://hz.iojbl.cn/gthsmxnmvd.html

ANALYZE TABLE users;
来源：http://hz.jlsjyb.cn/gtzppaiumz.html

[Q71] 查看建表语句
来源：http://hz.xuanzx.com/gtobftnxxc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nwbrower.top/gtilbnbftk.html

[Q72] 查看索引
来源：http://hz.gotoacloud.top/gtazrzgzov.html

SHOW INDEX FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtraqvsmwg.html

[Q73] 查看表状态
来源：http://hz.yongpay.top/gtxflshfeo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydjk.org.cn/gtqxahjeyo.html

[Q74] 强制使用索引
来源：http://hz.chenzaomai.com/gtvklmtjnv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zdqjudy.top/gtalpwvjki.html

[Q75] 日期格式化
来源：http://hz.kuanghao11.cn/gtzkrswhbi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.52xcode.cn/gttfczvjzr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yangfankeji.com/gtegukypds.html

[Q76] 按天统计
来源：http://hz.yj20258.top/gttdvhtztv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daria6918.cn/gtgazlgvcu.html

[Q77] 时间加减
来源：http://hz.zhongyouzk.top/gtaqppdovn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydjk.org.cn/gtxzqckzdu.html

[Q78] 当前时间
来源：http://hz.sweek.top/gtwnnnzyit.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuanzhike.top/gtdwladcki.html

[Q79] 字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtriiqzkhj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sysykeji.top/gtshuffdbo.html

[Q80] 字符串截取
来源：http://hz.guowangkeji.top/gtbtlcflei.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jlsjyb.cn/gtnboeyehs.html

[Q81] 字符串替换
来源：http://hz.hongshengwenyu.top/gtaaspptbq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shanyushiyangtech.top/gtcccdovap.html

[Q82] 字符长度与字节长度
来源：http://hz.jinghuilouyu.cn/gtlaztnaro.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydjk.org.cn/gtpopugqaz.html

[Q83] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtlztqrhjf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ehwqpu.com/gtunrceheu.html

[Q84] 去除首尾空格
来源：http://hz.ydzc1.top/gtniruzrue.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gtddvuxpxq.html

[Q85] 数值取整
来源：http://hz.wangdashe.top/gtjpkxswil.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cucudq.cn/gtmmkjhgmx.html

[Q86] 读取 JSON 字段
来源：http://hz.snrcjt.cn/gtjpwvxztr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.dianchejie.cn/gtdjaitnlj.html

[Q87] JSON 字段做条件
来源：http://hz.feifeiyinyue.top/gtospdxarq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.9152youxi.cn/gtpbsvjgla.html

[Q88] 行转列（条件聚合）
来源：http://hz.havefunace.top/gtibmpmlmr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.feifeiyinyue.top/gtwkgphnrj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.aizwys.cn/gtnowpfaik.html

[Q89] 判断表是否存在
来源：http://hz.dianchejie.cn/gtsmrtkook.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.kuanghao11.cn/gtpvsgmswv.html

[Q90] 生成序号列
来源：http://hz.c1oappe.top/gtgimleczz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.birdmap.top/gtspqnddon.html

================================================================================
来源：http://hz.yuxming.cn/gtnisnohbm.html

R. Bash 专题
来源：http://hz.cucudq.cn/gtevndutdi.html

================================================================================
来源：http://hz.sxryk.cn/gtulvadqpa.html

[R01] shebang 与严格模式
来源：http://hz.sweek.top/gtnunxoktq.html

#!/usr/bin/env bash
来源：http://hz.chenlongwang.top/gtzgxzjkfu.html

set -euo pipefail
来源：http://hz.cdnleiting.top/gtzwomanhl.html

[R02] 变量赋值与使用
来源：http://hz.tianlin.xyz/gtkewijvnp.html

name="Tom"; echo "$name"
来源：http://hz.cdnleiting.top/gtfwvtgvji.html

[R03] 只读变量
来源：http://hz.shanyushiyangtech.top/gtnpxbngli.html

readonly PI=3.14
来源：http://hz.quarkkingdee.top/gtxiovpxjq.html

[R04] 位置参数
来源：http://hz.xingfuxueyuan.xyz/gtyvlrlabj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.havefunace.top/gtoiesdqui.html

[R05] 参数默认值
来源：http://hz.cheryme.top/gtlxsfxflw.html

name="${1:-default}"
来源：http://hz.yueranfly.top/gtvtqtddaa.html

[R06] 判断命令是否存在
来源：http://hz.wangshuangyany.cn/gtemntjfus.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gttqjgayck.html

[R07] if 判断文件
来源：http://hz.ydjk.org.cn/gtudkfrdsv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.havefunace.top/gtunxdxkuv.html

[R08] 数值比较
来源：http://hz.xuetiantiany.cn/gtcdowjkzr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgfzy.top/gtjcaucjpu.html

[R09] 字符串比较
来源：http://hz.shanyushiyangkeji.top/gtwixvctrq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhiwuduotai.top/gtzhvuplxn.html

[R10] 正则匹配
来源：http://hz.jinqigufen.top/gttgkynmgy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cqqwz.cn/gtrmnozprd.html

[R11] case 多分支
来源：http://hz.sxryk.cn/gtzrkedvtp.html

case "$1" in
来源：http://hz.nanxinkj.top/gtcmlkezmk.html

start) echo "启动" ;;
来源：http://hz.daxiang520.top/gtcytaedec.html

stop)  echo "停止" ;;
来源：http://hz.tanke756.top/gtajulbdoi.html

*)     echo "未知命令" ;;
来源：http://hz.aibaodan.cn/gtcyokrmmp.html

esac
来源：http://hz.aibaodan.cn/gtxgmunqev.html

[R12] for 遍历文件
来源：http://hz.nwbrower.top/gtgabfrgbw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cheryme.top/gtvwvmnltq.html

[R13] for 计数循环
来源：http://hz.nanxinkj.top/gtbhwzvure.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tianlin.xyz/gtdqvuyata.html

[R14] C 风格 for
来源：http://hz.9152youxi.cn/gtxhcutsjf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xinyue.icu/gthvwijefu.html

[R15] while 逐行读文件
来源：http://hz.sweek.top/gtmybwezrp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtspyeikot.html

[R16] until 等待条件
来源：http://hz.guowangkeji.top/gtbfmchinh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hysaishi.cn/gtsmzjzpas.html

[R17] 数组定义与取值
来源：http://hz.fzhhl.top/gtrkexwkmr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sxryk.cn/gtjizqxuid.html

[R18] 遍历数组
来源：http://hz.ywan-chungtsiang.top/gtxpjzevms.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangshuangyany.cn/gtdnwtcctj.html

[R19] 数组长度
来源：http://hz.kuanghao11.cn/gtvhizdjnd.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtmcriplfy.html

[R20] 关联数组（字典）
来源：http://hz.yongpay.top/gtdmnrbrey.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigfzy.top/gtzzocqpgp.html

[R21] 字符串长度
来源：http://hz.zhengqikj.top/gtpokketww.html

echo "${#s}"
来源：http://hz.pycfn.com/gtbcalsdxp.html

[R22] 截取子串
来源：http://hz.gaohongyu789.top/gtvbaiqqpt.html

echo "${s:0:5}"
来源：http://hz.jlsjyb.cn/gtuenrquph.html

[R23] 字符串替换
来源：http://hz.gotoacloud.top/gtfehabtez.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shangyingyoupin.top/gtkwlkkxaj.html

[R24] 大小写转换
来源：http://hz.jlsjyb.cn/gtggfbjust.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ybcxt.top/gtukbvbjcr.html

[R25] 去后缀 / 去前缀
来源：http://hz.xingfuxueyuan.xyz/gtxaqnjiiq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ybcxt.top/gtdtqjoxbb.html

[R26] 命令替换
来源：http://hz.zhengqikj.top/gtbclupgbc.html

now=$(date +%F); echo "$now"
来源：http://hz.feifeiyinyue.top/gtrwdhzsth.html

[R27] 算术展开
来源：http://hz.chenjidiqi.icu/gtghdseqpi.html

echo $((1 + 2 * 3))
来源：http://hz.havefunace.top/gtsykiqpkz.html

[R28] 浮点运算
来源：http://hz.aibaodan.cn/gtfndmtkbg.html

echo "scale=2; 10/3" | bc
来源：http://hz.gzhubu.top/gtsitodaid.html

[R29] 定义函数
来源：http://hz.kuanghao11.cn/gtjjyvruun.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gotoacloud.top/gtbbufwnrd.html

[R30] 函数返回状态码
来源：http://hz.jlsjyb.cn/gtljahbbpx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.wangshuangyany.cn/gtfzervqld.html

[R31] 局部变量
来源：http://hz.yvedp.cn/gtmzamamnc.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangkeji.top/gtlwqcowte.html

[R32] 参数个数校验
来源：http://hz.0kj1m.cn/gtfasxphsp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ppjwa.cn/gtsexbtqep.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgfzy.top/gtdrswhfhk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shangyingyoupin.top/gtbdkdcvoe.html

[R34] 退出时清理
来源：http://hz.cucudq.cn/gtepczbtle.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtdsdorxca.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangkeji.top/gtcesorxer.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenjidiqi.icu/gtcnlzkggr.html

[R36] 并发执行多个任务
来源：http://hz.ivvv.top/gtvhdsqqzt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.andypj.xyz/gtwguisfih.html

[R37] 把输出赋给变量
来源：http://hz.zhongyouzk.top/gtqmxcddnj.html

files=$(ls -1)
来源：http://hz.ydjk.org.cn/gtbjacvtbn.html

[R38] 管道串联
来源：http://hz.cashguo.top/gtktmzkucc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuanzhike.top/gthsukvale.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtarpqoamj.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtwtglrafe.html

[R40] 追加写日志
来源：http://hz.daria6918.cn/gtnsxgttal.html

echo "log" >> out.log
来源：http://hz.yvedp.cn/gtwkiihntc.html

[R41] 丢弃输出
来源：http://hz.hywenlv.cn/gtvfnxcpss.html

cmd >/dev/null 2>&1
来源：http://hz.snrcjt.cn/gtwxqchjqd.html

[R42] 输入重定向
来源：http://hz.haohaochexian.top/gtslikhtec.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtbxkhvdrd.html

[R43] 按名字查找文件
来源：http://hz.tanke756.top/gtganavvip.html

find . -name "*.log" -type f
来源：http://hz.chenjidiqi.icu/gtkvkldqzh.html

[R44] 按修改时间查找
来源：http://hz.gaohongyu789.top/gtknmpqccm.html

find . -mtime -7 -type f
来源：http://hz.quarkkingdee.top/gtiflfhkdb.html

[R45] 批量删除
来源：http://hz.nwbrower.top/gtobnbwbsd.html

find . -name "*.tmp" -delete
来源：http://hz.xinyue.icu/gttiyvrwwo.html

[R46] 递归替换文件内容
来源：http://hz.svipenyu.cn/gtgbtsfsru.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhoulong.xyz/gtqjckayth.html

[R47] sed 单行替换
来源：http://hz.yongpay.top/gturliehii.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ybcxt.top/gtdwqpigzu.html

[R48] awk 取指定列
来源：http://hz.nanxuanxn.top/gtwsizpivf.html

awk '{print $1, $3}' a.txt
来源：http://hz.cheryme.top/gturbgozek.html

[R49] awk 带条件
来源：http://hz.vqdsnc.cn/gtzvcmahhf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhongyouzk.top/gttuzaxwyn.html

[R50] awk 求和
来源：http://hz.ehwqpu.com/gtynnxrydi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jianghu66.top/gtwjoioadi.html

[R51] 排序去重取前几
来源：http://hz.ydzc1.top/gtmlmuzbwz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yanxiufei.cn/gtcndzrigo.html

[R52] 统计行数
来源：http://hz.hysaishi.cn/gtqtgfwvhn.html

wc -l a.txt
来源：http://hz.cucudq.cn/gtsydgjhra.html

[R53] 查看文件头与实时尾
来源：http://hz.ybcxt.top/gttrtesjpz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yangfankeji.com/gtdecjhopd.html

[R54] 比较两个文件
来源：http://hz.hywenlv.cn/gtwmnakhpp.html

diff a.txt b.txt
来源：http://hz.pengpengdd.cyou/gtkqfltrfp.html

[R55] 压缩与解压
来源：http://hz.jinyuanbaomall.cn/gtrhawqzsc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yonumen.top/gtpwblgbna.html

[R56] 远程拷贝
来源：http://hz.ydjk.org.cn/gtszdpteol.html

scp file user@host:/path/
来源：http://hz.nanxuanxn.top/gtpinkgoey.html

[R57] 远程执行命令
来源：http://hz.yj202588.top/gtouhejmgk.html

ssh user@host 'uptime'
来源：http://hz.dianchejie.cn/gtyouwaolm.html

[R58] 下载文件
来源：http://hz.jqgufenzy.top/gtagbtbyrp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sxryk.cn/gtnuisqclu.html

[R59] 发 POST JSON
来源：http://hz.yuxming.cn/gtiaoktder.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yonumen.top/gtrsymkkyb.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangdashe.top/gtvappoumt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hfpthk.cn/gtadvjnodc.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gttzavddqq.html

df -h;  du -sh *
来源：http://hz.jqgufenzy.top/gtwxghuymm.html

[R62] 找最占空间的文件
来源：http://hz.wangshuangyany.cn/gtfaifiiqr.html

du -ah . | sort -rh | head -10
来源：http://hz.jyoumei.cn/gtmadncrmu.html

[R63] 内存与进程
来源：http://hz.hfpthk.cn/gtmgawnxxa.html

free -h;  ps aux | grep nginx
来源：http://hz.hongshengwenyu.top/gtyuasglxz.html

[R64] 结束进程
来源：http://hz.hfpthk.cn/gtoeiqverp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.feifeiyinyue.top/gtxwbhreem.html

[R65] 查看端口占用
来源：http://hz.nwbrower.top/gtwozylrbg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hammf.cn/gtbkzmotdc.html

[R66] 定时任务
来源：http://hz.zdqjudy.top/gtcgraqhts.html

crontab -e;  crontab -l
来源：http://hz.dianchejie.cn/gtdeioybmu.html

[R67] 生成随机十六进制串
来源：http://hz.gaohongyu789.top/gttpvhspuw.html

openssl rand -hex 16
来源：http://hz.birdmap.top/gtwqcxwece.html

[R68] 计算文件校验值
来源：http://hz.xziqi.cn/gtymkjlzdu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xziqi.cn/gttqggemjb.html

[R69] 生成随机密码
来源：http://hz.ehwqpu.com/gthrctoiht.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangtech.top/gtblwicsml.html

[R70] 时间戳与互转
来源：http://hz.sweek.top/gtugheppyf.html

date +%s;  date -d @1700000000
来源：http://hz.chenzaomai.com/gtqxdhvwcm.html

[R71] 日期格式化
来源：http://hz.snrcjt.cn/gtnynkprkj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinyuanbaomall.cn/gtmajarnli.html

[R72] 等待端口就绪
来源：http://hz.fengsongda.top/gtncoimgmn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gogol.net.cn/gttdyhmfbn.html

[R73] 分割大日志
来源：http://hz.jqgfzy.top/gtxbyyvhew.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gtdkuvzkqu.html

[R74] 批量重命名
来源：http://hz.nanxuanxn.top/gtrzjkthdt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtsgjmewyl.html

[R75] 导出环境变量
来源：http://hz.wangshuangyany.cn/gtwcuqdzty.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cqqwz.cn/gtuhepokat.html

[R76] 使用临时文件
来源：http://hz.xinyue.icu/gtcrqrwkzd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gthchjnhtu.html

[R77] 读取用户输入
来源：http://hz.mhx1999.top/gtldywccej.html

read -rp "请输入: " ans
来源：http://hz.shzxlz.cn/gtyexaqbmi.html

[R78] 交互式菜单
来源：http://hz.cqqwz.cn/gtaisntlhz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.c1oappe.top/gtggxkhjvx.html

[R79] 解析命令行选项
来源：http://hz.sweek.top/gtbfbpjrvf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.havefunace.top/gtaunvyfhx.html

[R80] 查看脚本执行耗时
来源：http://hz.xziqi.cn/gtlgnchcti.html

time ./run.sh
来源：http://hz.ywan-chungtsiang.top/gtaobfweln.html

================================================================================
来源：http://hz.dianchejie.cn/gtnjnygxpg.html

S. C / C++ 专题
来源：http://hz.smart0.xyz/gtbqiodsvi.html

================================================================================
来源：http://hz.xylfe.cn/gtwponlgns.html

[S01] C：Hello World
来源：http://hz.sweek.top/gtnigcdodx.html

#include <stdio.h>
来源：http://hz.sufxvd.cn/gtshjigccp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenlongwang.top/gtcikoybav.html

[S02] C：变量与格式化输出
来源：http://hz.hfpthk.cn/gtfgfjqomq.html

int a = 10; printf("%d\n", a);
来源：http://hz.xziqi.cn/gthygtbejg.html

[S03] C：读入整数
来源：http://hz.gaohongyu789.top/gtnapqyryh.html

int x; scanf("%d", &x);
来源：http://hz.gzhubu.top/gtopvpyivn.html

[S04] C：字符串复制
来源：http://hz.dianchejie.cn/gtjbquglzj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jqgufenzy.top/gtcjjjhhzc.html

[S05] C：字符串长度
来源：http://hz.yj20258888.top/gtofjpjupn.html

strlen(s)
来源：http://hz.jlsjyb.cn/gtjqlgxalx.html

[S06] C：字符串比较
来源：http://hz.jinghuilouyu.cn/gtjuwpwpij.html

strcmp(a, b) == 0
来源：http://hz.yuanzhike.top/gtqvjupgii.html

[S07] C：数组遍历求和
来源：http://hz.mhx1999.top/gtvvnvtsuz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gtwhdgxidb.html

[S08] C：动态内存分配与释放
来源：http://hz.gaohongyu789.top/gtchjiabhw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sxryk.cn/gthjnfgqoh.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gthxymvjyj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aizwys.cn/gtaasuwncw.html

[S10] C：指针与解引用
来源：http://hz.kuanghao11.cn/gtpomkmzbh.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtxxnofpks.html

[S11] C：逐行读文件
来源：http://hz.hnxiangtu.top/gttpexjpsx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuetiantiany.cn/gtavebseyf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fzhhl.top/gtvwbjmboo.html

fclose(f);
来源：http://hz.zhengqikj.top/gtsypdfyis.html

[S12] C：写文件
来源：http://hz.zhiwuduotai.top/gttkvgmwxt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.havefunace.top/gtlooyyvti.html

[S13] C：宏定义
来源：http://hz.bjfxy.top/gtwltnejhi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj20258.top/gtluhxfeug.html

[S14] C：枚举
来源：http://hz.nanxuanxn.top/gtwsydgxvw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.52xcode.cn/gtjwldfgky.html

[S15] C：类型转换
来源：http://hz.zhiwuduotai.top/gtgzzozagn.html

(double) a / b
来源：http://hz.nanxinkj.top/gtiopkaqjo.html

[S16] C：位操作置位
来源：http://hz.gzhubu.top/gtgtajdqvs.html

x |= (1 << 3);
来源：http://hz.gaohongyu789.top/gtwbdmnxdr.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258888.top/gtlefkvyns.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.mhx1999.top/gtmumpcpxv.html

[S18] C：命令行参数
来源：http://hz.ehwqpu.com/gtgibadesb.html

int main(int argc, char **argv)
来源：http://hz.ydzc1.top/gtujwzwdgx.html

[S19] C：快速排序
来源：http://hz.nwbrower.top/gtdynejfai.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gzhubu.top/gtkhhcibaq.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gtwaybnnbi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.meibo888.top/gtoahgknrx.html

[S21] C：字符类别判断
来源：http://hz.hysaishi.cn/gtkgdnflgq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gzhubu.top/gttthvyrxt.html

[S22] C：字符串转数字
来源：http://hz.gaohongyu789.top/gteenvjmnk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hfpthk.cn/gtihoekbvp.html

[S23] C：随机数
来源：http://hz.xylfe.cn/gtrrbfjqub.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.birdmap.top/gtrflrcief.html

[S24] C：获取本地时间
来源：http://hz.jlsjyb.cn/gtjjzuqhap.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhiwuduotai.top/gtrlskkwhl.html

[S25] C：内存拷贝
来源：http://hz.jyoumei.cn/gtgwtrziam.html

memcpy(dst, src, n);
来源：http://hz.xylfe.cn/gtearkumap.html

[S26] C：内存清零
来源：http://hz.sweek.top/gtgaaqnmde.html

memset(a, 0, sizeof a);
来源：http://hz.quarkkingdee.top/gtfziugquw.html

[S27] C：定义常量
来源：http://hz.guowangkeji.top/gtwcqunyci.html

const double PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtjopenufm.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtsutqhihw.html


<!-- 参考信息 -->