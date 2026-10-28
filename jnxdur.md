代发 wailian999

[Q65] 回滚事务
来源：http://hz.tian-w.cn/gtsoqlvyyy.html

ROLLBACK;
来源：http://hz.hnqzz.top/gthtpyfdvz.html

[Q66] 行锁查询
来源：http://hz.zhengqikj.top/gtpblnspea.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fengsongda.top/gtmrlstiuf.html

[Q67] 设置隔离级别
来源：http://hz.dianchejie.cn/gtjqeyfkid.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgufenzy.top/gtukcfddlb.html

[Q68] 保存点
来源：http://hz.yuanzhike.top/gttbvxtnnn.html

SAVEPOINT sp1;
来源：http://hz.zhaomingkeji.xyz/gtewerkhlr.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gtfkrfkvfc.html

[Q69] 查看执行计划
来源：http://hz.zdqjudy.top/gtiaruuqqx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhaomingkeji.xyz/gthoggytse.html

[Q70] 更新统计信息
来源：http://hz.gogol.net.cn/gtsbiphbvn.html

ANALYZE TABLE users;
来源：http://hz.aizwys.cn/gtxryzbpnh.html

[Q71] 查看建表语句
来源：http://hz.zhongyouzk.top/gtypepgorg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.quarkkingdee.top/gtjsroczgd.html

[Q72] 查看索引
来源：http://hz.zhaomingkeji.xyz/gtzocgbigb.html

SHOW INDEX FROM users;
来源：http://hz.ppjwa.cn/gttslmarkg.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangkeji.top/gtyiruibkn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zycfv.cn/gtgerrvspi.html

[Q74] 强制使用索引
来源：http://hz.zhongyouzk.top/gtnsvnipfn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.havefunace.top/gtbpkvrhwz.html

[Q75] 日期格式化
来源：http://hz.yj20258.top/gtfuwvfjsu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sxryk.cn/gtrpuebfqw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhijiandao.cn/gtvdezlnuz.html

[Q76] 按天统计
来源：http://hz.shanyushiyangtech.top/gtyuaqmwrx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.9152youxi.cn/gteaabbcev.html

[Q77] 时间加减
来源：http://hz.redwolf501.top/gtywxillbb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtrwknzkjx.html

[Q78] 当前时间
来源：http://hz.cashguo.top/gtmpdskhyt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.redwolf501.top/gtjutgpjqp.html

[Q79] 字符串拼接
来源：http://hz.sxryk.cn/gtxqlaiuga.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtiwwhqldj.html

[Q80] 字符串截取
来源：http://hz.smart0.xyz/gtblzrqcmf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.mhx1999.top/gthhesxovf.html

[Q81] 字符串替换
来源：http://hz.sysykeji.top/gtflhtkbqw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.316326.xyz/gtkercdtux.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxuanxn.top/gtpejtyitm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yonumen.top/gtcgglmwhm.html

[Q83] 大小写转换
来源：http://hz.tian-w.cn/gtmatyikiu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hnxiangtu.top/gtjneefqkv.html

[Q84] 去除首尾空格
来源：http://hz.xuetiantiany.cn/gthfrfedpi.html

SELECT TRIM(name) FROM users;
来源：http://hz.0kj1m.cn/gtphyleupn.html

[Q85] 数值取整
来源：http://hz.hfpthk.cn/gtinghqdao.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.meibo888.top/gtljfrllwc.html

[Q86] 读取 JSON 字段
来源：http://hz.bjfxy.top/gtikgnlsbn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenzaomai.com/gtedpolxmk.html

[Q87] JSON 字段做条件
来源：http://hz.feifeiyinyue.top/gtqgypozfh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cdnleiting.top/gtbeajqbtm.html

[Q88] 行转列（条件聚合）
来源：http://hz.tianlin.xyz/gtqwgruqro.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jlsjyb.cn/gtwncnylye.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ppjwa.cn/gtzcowqwpx.html

[Q89] 判断表是否存在
来源：http://hz.redwolf501.top/gtrzcsxdia.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gaohongyu789.top/gtkpjmrwhk.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gtfmiprfup.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuanzhike.top/gtcxvxzyzw.html

================================================================================
来源：http://hz.gogol.net.cn/gtbpuqayek.html

R. Bash 专题
来源：http://hz.jianghu66.top/gtusdgawza.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtafbfwdvv.html

[R01] shebang 与严格模式
来源：http://hz.316326.xyz/gtpqoytnws.html

#!/usr/bin/env bash
来源：http://hz.yj20258.top/gtpfyteuyc.html

set -euo pipefail
来源：http://hz.hongshengwenyu.top/gtqiwgeuia.html

[R02] 变量赋值与使用
来源：http://hz.yongpay.top/gthsufmihp.html

name="Tom"; echo "$name"
来源：http://hz.havefunace.top/gtzobogxmz.html

[R03] 只读变量
来源：http://hz.hnqzz.top/gtbtsxyyee.html

readonly PI=3.14
来源：http://hz.yj202588.top/gtngmkdwiu.html

[R04] 位置参数
来源：http://hz.jinqigfzy.top/gtpifpvwps.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangtech.top/gtojmpgfdi.html

[R05] 参数默认值
来源：http://hz.zhijiandao.cn/gtnzuxffjv.html

name="${1:-default}"
来源：http://hz.redwolf501.top/gtpaiscnns.html

[R06] 判断命令是否存在
来源：http://hz.nwbrower.top/gthtivkzby.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.redwolf501.top/gtvmgvsyih.html

[R07] if 判断文件
来源：http://hz.gzhubu.top/gtuftwnkmc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hfpthk.cn/gtkhkgvekg.html

[R08] 数值比较
来源：http://hz.jinqigfzy.top/gtvgiiagth.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gogol.net.cn/gttetutqoq.html

[R09] 字符串比较
来源：http://hz.tianlin.xyz/gtbrpfdeup.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zycfv.cn/gtfmqdntjk.html

[R10] 正则匹配
来源：http://hz.jianghu66.top/gtjusndmqw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shanyushiyangtech.top/gtoucvwypy.html

[R11] case 多分支
来源：http://hz.ppjwa.cn/gtscuhkmma.html

case "$1" in
来源：http://hz.xingfuxueyuan.xyz/gtieaiiblr.html

start) echo "启动" ;;
来源：http://hz.shzxlz.cn/gtuqtljxol.html

stop)  echo "停止" ;;
来源：http://hz.iojbl.cn/gtoocxcmwc.html

*)     echo "未知命令" ;;
来源：http://hz.iojbl.cn/gtzfrxuyjf.html

esac
来源：http://hz.shzxlz.cn/gtuewonzlj.html

[R12] for 遍历文件
来源：http://hz.svipenyu.cn/gtwrwfxhso.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cqqwz.cn/gtrormldiv.html

[R13] for 计数循环
来源：http://hz.jlsjyb.cn/gtmknstbqz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hywenlv.cn/gtdwwebccr.html

[R14] C 风格 for
来源：http://hz.gogol.net.cn/gtkrwyieai.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj202588.top/gttsrubvov.html

[R15] while 逐行读文件
来源：http://hz.wangdashe.top/gtgkbknzur.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fengsongda.top/gttcrnsaic.html

[R16] until 等待条件
来源：http://hz.dashuyun.cn/gtstcvasfn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xingfuxueyuan.xyz/gtuocrnzjl.html

[R17] 数组定义与取值
来源：http://hz.hnqzz.top/gtsnepfsfl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydzc1.top/gtbyvffwcx.html

[R18] 遍历数组
来源：http://hz.yanxiufei.cn/gtdlqrkttx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhoulong.xyz/gtfcjduslt.html

[R19] 数组长度
来源：http://hz.zhongyouzk.top/gtiabmgmxh.html

echo "${#arr[@]}"
来源：http://hz.hfpthk.cn/gtwczlmska.html

[R20] 关联数组（字典）
来源：http://hz.sweek.top/gtyiytgvem.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.chenlongwang.top/gtteupjjae.html

[R21] 字符串长度
来源：http://hz.yuanzhike.top/gtetcmgyxr.html

echo "${#s}"
来源：http://hz.dianchejie.cn/gtclqblwef.html

[R22] 截取子串
来源：http://hz.aizwys.cn/gtpespajba.html

echo "${s:0:5}"
来源：http://hz.yj20258.top/gtmmhbbjfz.html

[R23] 字符串替换
来源：http://hz.pycfn.com/gttunjtbbs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.aibaodan.cn/gtishrnxbr.html

[R24] 大小写转换
来源：http://hz.yonumen.top/gtbudbumlr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ivvv.top/gtrbyvhtbh.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gtzokoyxdn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hfpthk.cn/gtkoinehjy.html

[R26] 命令替换
来源：http://hz.zycfv.cn/gtyeoyerto.html

now=$(date +%F); echo "$now"
来源：http://hz.sweek.top/gtxvzscrtu.html

[R27] 算术展开
来源：http://hz.yuanzhike.top/gtnupeumen.html

echo $((1 + 2 * 3))
来源：http://hz.zycfv.cn/gtlcgwhoxf.html

[R28] 浮点运算
来源：http://hz.tian-w.cn/gtxcmaptia.html

echo "scale=2; 10/3" | bc
来源：http://hz.cashguo.top/gtgonoonzf.html

[R29] 定义函数
来源：http://hz.sweek.top/gtuypjjfyy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xylfe.cn/gtgyqsikfr.html

[R30] 函数返回状态码
来源：http://hz.jyoumei.cn/gtbtwfcaqj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nwbrower.top/gtqrrpwtuv.html

[R31] 局部变量
来源：http://hz.zhixingplan.top/gtacspufhl.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinghuilouyu.cn/gttsszwbnp.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gtbnxcvztb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dashuyun.cn/gtaxjdmjfd.html

[R33] 捕获错误并提示行号
来源：http://hz.ehwqpu.com/gtbvutcrib.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhengqikj.top/gtfaaevgmg.html

[R34] 退出时清理
来源：http://hz.0kj1m.cn/gtzlwzhsdp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gthdmecskg.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtkywmzpoi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cheryme.top/gtnfmzhkvu.html

[R36] 并发执行多个任务
来源：http://hz.jyoumei.cn/gtbcqvlpma.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gogol.net.cn/gtqrwdwunu.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangkeji.top/gtptcxqjfh.html

files=$(ls -1)
来源：http://hz.zhijiandao.cn/gtspnlzidg.html

[R38] 管道串联
来源：http://hz.tanke756.top/gtkziljotf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ivvv.top/gtbpqtropz.html

[R39] 重定向标准输出与错误
来源：http://hz.yueranfly.top/gtehwliqbv.html

cmd > out.log 2>&1
来源：http://hz.dianchejie.cn/gtifigyspk.html

[R40] 追加写日志
来源：http://hz.jinqigfzy.top/gtsypyzdyf.html

echo "log" >> out.log
来源：http://hz.hnxiangtu.top/gtdasikhvk.html

[R41] 丢弃输出
来源：http://hz.yj20258.top/gtlprcsqtz.html

cmd >/dev/null 2>&1
来源：http://hz.andypj.xyz/gtgmdyitxq.html

[R42] 输入重定向
来源：http://hz.sweek.top/gtsvhuxiar.html

wc -l < a.txt
来源：http://hz.yj20258888.top/gtyuegluxm.html

[R43] 按名字查找文件
来源：http://hz.jqgufenzy.top/gtvotbigil.html

find . -name "*.log" -type f
来源：http://hz.yongpay.top/gtnllnbbwg.html

[R44] 按修改时间查找
来源：http://hz.hammf.cn/gtdizypzmo.html

find . -mtime -7 -type f
来源：http://hz.xinyue.icu/gtqijqiztt.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtojzcplxa.html

find . -name "*.tmp" -delete
来源：http://hz.aizwys.cn/gtqjajkhaq.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gticatbuiy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.fzhhl.top/gtilmqutwp.html

[R47] sed 单行替换
来源：http://hz.jinyuanbaomall.cn/gtvxtypzqu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dashuyun.cn/gtomdzasbq.html

[R48] awk 取指定列
来源：http://hz.jianghu66.top/gtzhebtfsg.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtahvqifgn.html

[R49] awk 带条件
来源：http://hz.jlsjyb.cn/gtezlbylbp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pycfn.com/gttwfgnvfb.html

[R50] awk 求和
来源：http://hz.wangdashe.top/gteqribeyl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.havefunace.top/gtvmbgctow.html

[R51] 排序去重取前几
来源：http://hz.ehwqpu.com/gtiermawdo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tanke756.top/gtqqtnjana.html

[R52] 统计行数
来源：http://hz.fzhhl.top/gtevpdewtr.html

wc -l a.txt
来源：http://hz.sufxvd.cn/gtjcydbpxb.html

[R53] 查看文件头与实时尾
来源：http://hz.dashuyun.cn/gtqalvxeux.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sxryk.cn/gtbujrtksq.html

[R54] 比较两个文件
来源：http://hz.yuanzhike.top/gtgcwsjnna.html

diff a.txt b.txt
来源：http://hz.gzhubu.top/gtjaywxtyr.html

[R55] 压缩与解压
来源：http://hz.guowangkeji.top/gtzveksczo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangdashe.top/gthlcgkomg.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtmuugvrrc.html

scp file user@host:/path/
来源：http://hz.yj20258888.top/gtsojcldrg.html

[R57] 远程执行命令
来源：http://hz.hysaishi.cn/gtoougwstb.html

ssh user@host 'uptime'
来源：http://hz.yonumen.top/gtbbnajzzc.html

[R58] 下载文件
来源：http://hz.guowangkeji.top/gtklrndsaj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sysykeji.top/gtmpvtpzrr.html

[R59] 发 POST JSON
来源：http://hz.dianchejie.cn/gtvyhsuxnr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.fengsongda.top/gtgifeteut.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenzaomai.com/gtzfyuhidc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zdqjudy.top/gtjlubigdc.html

[R61] 磁盘占用
来源：http://hz.sxryk.cn/gtolpuortg.html

df -h;  du -sh *
来源：http://hz.sweek.top/gtvuckprlh.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangtech.top/gtwhfitjrv.html

du -ah . | sort -rh | head -10
来源：http://hz.haohaochexian.top/gtjjrssezk.html

[R63] 内存与进程
来源：http://hz.zdqjudy.top/gtnhhcnoqw.html

free -h;  ps aux | grep nginx
来源：http://hz.yangfankeji.com/gtecvimezj.html

[R64] 结束进程
来源：http://hz.wangdashe.top/gtsjlgfkdo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinyuanbaomall.cn/gtgesztvkk.html

[R65] 查看端口占用
来源：http://hz.yj20258888.top/gtjjucmslw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuxming.cn/gtnankztof.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtdfeqrovu.html

crontab -e;  crontab -l
来源：http://hz.cashguo.top/gtbjbxuhtl.html

[R67] 生成随机十六进制串
来源：http://hz.ehwqpu.com/gtfsvarfmv.html

openssl rand -hex 16
来源：http://hz.ppjwa.cn/gtwqdrkoff.html

[R68] 计算文件校验值
来源：http://hz.316326.xyz/gtprjpxiot.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jlsjyb.cn/gtikbjckdj.html

[R69] 生成随机密码
来源：http://hz.tian-w.cn/gtuxtmhfnf.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinqigfzy.top/gtiwbshect.html

[R70] 时间戳与互转
来源：http://hz.jinghuilouyu.cn/gtxipkwxgh.html

date +%s;  date -d @1700000000
来源：http://hz.tianlin.xyz/gtxzxlzrat.html

[R71] 日期格式化
来源：http://hz.nwbrower.top/gtqtmjrrfe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuanzhike.top/gtsmqarppt.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gtnelxynpz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yueranfly.top/gtjhkcyurj.html

[R73] 分割大日志
来源：http://hz.xuetiantiany.cn/gtqwixrqkg.html

split -l 1000 big.log part_
来源：http://hz.ppjwa.cn/gtbldakcos.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gtefgctzwq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yuanzhike.top/gtdiecrtpn.html

[R75] 导出环境变量
来源：http://hz.zhongyouzk.top/gtvzzscfka.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigufen.top/gtcsuqyrvi.html

[R76] 使用临时文件
来源：http://hz.jlsjyb.cn/gtnivgplvy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtawuwnacn.html

[R77] 读取用户输入
来源：http://hz.nanxinkj.top/gtgbmgefnh.html

read -rp "请输入: " ans
来源：http://hz.xinyue.icu/gtftnidzax.html

[R78] 交互式菜单
来源：http://hz.sweek.top/gtwihlsunz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ivvv.top/gtngzjbxcg.html

[R79] 解析命令行选项
来源：http://hz.cucudq.cn/gtmcxdlasm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.guowangkeji.top/gtppbafyfc.html

[R80] 查看脚本执行耗时
来源：http://hz.redwolf501.top/gtjaiozefl.html

time ./run.sh
来源：http://hz.nanxinkj.top/gtwmbbenqp.html

================================================================================
来源：http://hz.tian-w.cn/gtdecttbyw.html

S. C / C++ 专题
来源：http://hz.zhixingplan.top/gthknvgdpk.html

================================================================================
来源：http://hz.sxryk.cn/gtwzfpuwgn.html

[S01] C：Hello World
来源：http://hz.smart0.xyz/gtusdhswwg.html

#include <stdio.h>
来源：http://hz.yj20258888.top/gtnxfkdfgz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gaohongyu789.top/gtwuuywgxz.html

[S02] C：变量与格式化输出
来源：http://hz.hnqzz.top/gtddtpwcqp.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgfzy.top/gtqrpkiozb.html

[S03] C：读入整数
来源：http://hz.jiagoushi.top/gtuxpcrhmp.html

int x; scanf("%d", &x);
来源：http://hz.ppjwa.cn/gtuclzlkdj.html

[S04] C：字符串复制
来源：http://hz.ybcxt.top/gthpdxbhel.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxuanxn.top/gtwmortphc.html

[S05] C：字符串长度
来源：http://hz.zhengqikj.top/gttqglgqzr.html

strlen(s)
来源：http://hz.meibo888.top/gtujwvarmg.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gttwlahtfn.html

strcmp(a, b) == 0
来源：http://hz.cqqwz.cn/gtsseggzzf.html

[S07] C：数组遍历求和
来源：http://hz.sysykeji.top/gtroqitweo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aizwys.cn/gtxsyhxdgv.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258888.top/gtthkeovtp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhixingplan.top/gtsrgtbhuo.html

[S09] C：结构体定义与初始化
来源：http://hz.wangshuangyany.cn/gtduvuafgj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtvlmwihcq.html

[S10] C：指针与解引用
来源：http://hz.hysaishi.cn/gtfmmxcgkr.html

int *p = &a;  *p = 5;
来源：http://hz.jiagoushi.top/gtgvwlfavb.html

[S11] C：逐行读文件
来源：http://hz.kuanghao11.cn/gtrfxruogc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yuanzhike.top/gtkvjygsyc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnqzz.top/gtwiqieagm.html

fclose(f);
来源：http://hz.zycfv.cn/gtkzdclzng.html

[S12] C：写文件
来源：http://hz.yanxiufei.cn/gtsknworrq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuxming.cn/gtdughycau.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtjgngmcsc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.svipenyu.cn/gtdvruplwl.html

[S14] C：枚举
来源：http://hz.xingfuxueyuan.xyz/gtvbmxtqor.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xylfe.cn/gtrbzuckfr.html

[S15] C：类型转换
来源：http://hz.316326.xyz/gtdssundqz.html

(double) a / b
来源：http://hz.9152youxi.cn/gtregribdb.html

[S16] C：位操作置位
来源：http://hz.yueranfly.top/gtlmrkpayy.html

x |= (1 << 3);
来源：http://hz.yj20258888.top/gthhgqhwao.html

[S17] C：安全拼接字符串
来源：http://hz.chenlongwang.top/gtybxaovlt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.svipenyu.cn/gtkpynoaxv.html

[S18] C：命令行参数
来源：http://hz.jyoumei.cn/gtewdjayfn.html

int main(int argc, char **argv)
来源：http://hz.jyoumei.cn/gtylxjcuvl.html

[S19] C：快速排序
来源：http://hz.9152youxi.cn/gtibkbaxow.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtmesksomy.html

[S20] C：二分查找
来源：http://hz.zhaomingkeji.xyz/gthmcndsar.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtacqgkjkw.html

[S21] C：字符类别判断
来源：http://hz.jinyuanbaomall.cn/gtlfhvndwr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shzxlz.cn/gtenhypbfe.html

[S22] C：字符串转数字
来源：http://hz.ydzc1.top/gtwpkhybwu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinqigfzy.top/gtudysjhdb.html

[S23] C：随机数
来源：http://hz.316326.xyz/gtaydhgjhq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenjidiqi.icu/gtdixerkaj.html

[S24] C：获取本地时间
来源：http://hz.yanxiufei.cn/gtpjgwojvj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daria6918.cn/gtrlfqtfzi.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtvarwchqw.html

memcpy(dst, src, n);
来源：http://hz.ehwqpu.com/gtdlrzapuw.html

[S26] C：内存清零
来源：http://hz.zhaomingkeji.xyz/gthkzdwooz.html

memset(a, 0, sizeof a);
来源：http://hz.jianghu66.top/gtwljafidw.html

[S27] C：定义常量
来源：http://hz.yanxiufei.cn/gtfmrwxllg.html

const double PI = 3.14159;
来源：http://hz.pycfn.com/gtmvcixrnd.html

[S28] C：静态变量
来源：http://hz.xziqi.cn/gtvaslqoks.html

static int counter = 0;
来源：http://hz.cheryme.top/gtpdxdvjmv.html

[S29] C：变参函数
来源：http://hz.0kj1m.cn/gtybdjvqow.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgufenzy.top/gtwgyphihp.html

[S30] C：头文件保护
来源：http://hz.yangfankeji.com/gtbuzakylq.html

#ifndef X_H
来源：http://hz.sufxvd.cn/gtfstfynob.html

#define X_H
来源：http://hz.jinyuanbaomall.cn/gtqstfuaub.html

#endif
来源：http://hz.daxiang520.top/gtocbyoomk.html

[S31] C++：Hello World
来源：http://hz.jyoumei.cn/gthqyktigb.html

#include <iostream>
来源：http://hz.tian-w.cn/gtksafkomm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dashuyun.cn/gtlyukjqbu.html

[S32] C++：字符串
来源：http://hz.cqqwz.cn/gtqohayrsh.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigufen.top/gtkspmcquv.html

[S33] C++：vector 增删
来源：http://hz.jinyuanbaomall.cn/gtyshmnpxh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aizwys.cn/gtbknhlktc.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gtfqxfimys.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sxryk.cn/gtkwqafdrj.html


<!-- 参考信息 -->