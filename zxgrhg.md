代发 wailian999

[Q65] 回滚事务
来源：http://hz.sufxvd.cn/gtbbpielhb.html

ROLLBACK;
来源：http://hz.andypj.xyz/gtbpqozobe.html

[Q66] 行锁查询
来源：http://hz.dianchejie.cn/gtasmyfcwf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gaohongyu789.top/gtunxrhkfd.html

[Q67] 设置隔离级别
来源：http://hz.fzhhl.top/gtoqvnbcbx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hfpthk.cn/gttbpooggr.html

[Q68] 保存点
来源：http://hz.hongshengwenyu.top/gtvdklsxjq.html

SAVEPOINT sp1;
来源：http://hz.ydzc1.top/gtopebwhbd.html

ROLLBACK TO sp1;
来源：http://hz.sxryk.cn/gtexjtksli.html

[Q69] 查看执行计划
来源：http://hz.haohaochexian.top/gttlcfvrkv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhaomingkeji.xyz/gtrlopthnb.html

[Q70] 更新统计信息
来源：http://hz.yj202588.top/gturzeluav.html

ANALYZE TABLE users;
来源：http://hz.jianghu66.top/gtrvjxghhh.html

[Q71] 查看建表语句
来源：http://hz.ywan-chungtsiang.top/gtsmehgpzu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sysykeji.top/gtwcfzvywc.html

[Q72] 查看索引
来源：http://hz.yuanzhike.top/gtiriifort.html

SHOW INDEX FROM users;
来源：http://hz.andypj.xyz/gtiqxrmogt.html

[Q73] 查看表状态
来源：http://hz.sysykeji.top/gtckmgxywy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sysykeji.top/gtmwjkcoan.html

[Q74] 强制使用索引
来源：http://hz.hnqzz.top/gtugjmpfyg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sufxvd.cn/gtvdkwxkkr.html

[Q75] 日期格式化
来源：http://hz.cheryme.top/gtgambhqyv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jqgfzy.top/gtqpjwidfc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtjqcurntk.html

[Q76] 按天统计
来源：http://hz.meibo888.top/gtmonyovxq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.andypj.xyz/gtrgjxhaxi.html

[Q77] 时间加减
来源：http://hz.feifeiyinyue.top/gttkirqgwm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.smart0.xyz/gtsxovwgas.html

[Q78] 当前时间
来源：http://hz.yongpay.top/gtxeinqxjx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hammf.cn/gteeygapan.html

[Q79] 字符串拼接
来源：http://hz.yj202588.top/gtluwdcixx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cdnleiting.top/gtxxwafxnc.html

[Q80] 字符串截取
来源：http://hz.snrcjt.cn/gtgmhfzjbe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj20258.top/gtbgdqeatu.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gtqhfpsglv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ywan-chungtsiang.top/gtxpoysenw.html

[Q82] 字符长度与字节长度
来源：http://hz.mhx1999.top/gthirdvmxz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ehwqpu.com/gtxrjgidvs.html

[Q83] 大小写转换
来源：http://hz.pycfn.com/gtpgdafruu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gotoacloud.top/gtdfxofddv.html

[Q84] 去除首尾空格
来源：http://hz.iojbl.cn/gtltakooya.html

SELECT TRIM(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtcbkbcuyc.html

[Q85] 数值取整
来源：http://hz.feifeiyinyue.top/gtqvxrtvpv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jlsjyb.cn/gtegxkygpr.html

[Q86] 读取 JSON 字段
来源：http://hz.cheryme.top/gtrtinxmlg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.52xcode.cn/gtbmajwqid.html

[Q87] JSON 字段做条件
来源：http://hz.ywan-chungtsiang.top/gtklfzqzlx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxuanxn.top/gteawxvefz.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gtjeacrqvh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhijiandao.cn/gtrhunuvdi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daria6918.cn/gtgpfmzays.html

[Q89] 判断表是否存在
来源：http://hz.yanxiufei.cn/gtpkifsahe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gzhubu.top/gtcjspwkse.html

[Q90] 生成序号列
来源：http://hz.haohaochexian.top/gtinrlliju.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhixingplan.top/gtoqxaupib.html

================================================================================
来源：http://hz.yangfankeji.com/gtuyidqgza.html

R. Bash 专题
来源：http://hz.zhixingplan.top/gtqehjnoqs.html

================================================================================
来源：http://hz.nanxuanxn.top/gtsrxmlbzr.html

[R01] shebang 与严格模式
来源：http://hz.vqdsnc.cn/gtktqddbyh.html

#!/usr/bin/env bash
来源：http://hz.316326.xyz/gtmegwzaxt.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtdhcmutuf.html

[R02] 变量赋值与使用
来源：http://hz.hysaishi.cn/gtaqezhqeq.html

name="Tom"; echo "$name"
来源：http://hz.sxryk.cn/gtltlqsnmj.html

[R03] 只读变量
来源：http://hz.daxiang520.top/gtrvscjzpe.html

readonly PI=3.14
来源：http://hz.svipenyu.cn/gtgllqvxfh.html

[R04] 位置参数
来源：http://hz.meibo888.top/gtmyopzftf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj202588.top/gtgkrpicqo.html

[R05] 参数默认值
来源：http://hz.jqgfzy.top/gtsnlusrkb.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gtsgeofint.html

[R06] 判断命令是否存在
来源：http://hz.nanxinkj.top/gtwzuxfmko.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtfejnwdfs.html

[R07] if 判断文件
来源：http://hz.yuxming.cn/gtdzyrvbyi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.0kj1m.cn/gtbnjazgvc.html

[R08] 数值比较
来源：http://hz.yj20258.top/gtszjuuqkp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.redwolf501.top/gtjqhrbwju.html

[R09] 字符串比较
来源：http://hz.mhx1999.top/gtvtaussue.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tian-w.cn/gtqtcfbkzq.html

[R10] 正则匹配
来源：http://hz.cdnleiting.top/gthenntuur.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dianchejie.cn/gtbawusvev.html

[R11] case 多分支
来源：http://hz.yonumen.top/gtgpzthcio.html

case "$1" in
来源：http://hz.hfpthk.cn/gtarelkqsj.html

start) echo "启动" ;;
来源：http://hz.jqgufenzy.top/gtnmfrgwrv.html

stop)  echo "停止" ;;
来源：http://hz.shuidangran.top/gtcwqyijla.html

*)     echo "未知命令" ;;
来源：http://hz.yangfankeji.com/gtanmurcpm.html

esac
来源：http://hz.yongpay.top/gtpbvknalb.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gtbpmrqbpj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aibaodan.cn/gtzhwhhmbr.html

[R13] for 计数循环
来源：http://hz.guannengcc.top/gtmngzilfw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ivvv.top/gtphmbpxgz.html

[R14] C 风格 for
来源：http://hz.cdnleiting.top/gtgspffofs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jiagoushi.top/gtecmjjgca.html

[R15] while 逐行读文件
来源：http://hz.guowangkeji.top/gtvllkxoom.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigfzy.top/gtfuhpbpex.html

[R16] until 等待条件
来源：http://hz.iojbl.cn/gtpkakarmq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.52xcode.cn/gtasitalkr.html

[R17] 数组定义与取值
来源：http://hz.fzhhl.top/gtwafkjzpy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gttgvlpyxb.html

[R18] 遍历数组
来源：http://hz.cashguo.top/gtmlbhtdgx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nwbrower.top/gtlluupbji.html

[R19] 数组长度
来源：http://hz.fengsongda.top/gtmuxleevs.html

echo "${#arr[@]}"
来源：http://hz.0kj1m.cn/gtmgngffqn.html

[R20] 关联数组（字典）
来源：http://hz.fengsongda.top/gtszrmkkgl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.havefunace.top/gtvjxhmsat.html

[R21] 字符串长度
来源：http://hz.ydjk.org.cn/gtptolunwg.html

echo "${#s}"
来源：http://hz.yvedp.cn/gttrxofngs.html

[R22] 截取子串
来源：http://hz.jianghu66.top/gtnzxofkev.html

echo "${s:0:5}"
来源：http://hz.zycfv.cn/gtbykhggsd.html

[R23] 字符串替换
来源：http://hz.jianghu66.top/gtrrbjztha.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sysykeji.top/gtvqhqphqa.html

[R24] 大小写转换
来源：http://hz.zhixingplan.top/gtrmqtrioq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.52xcode.cn/gtmoskwdps.html

[R25] 去后缀 / 去前缀
来源：http://hz.smart0.xyz/gtwpgkktrx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258.top/gtjmvnzulh.html

[R26] 命令替换
来源：http://hz.zdqjudy.top/gtvzuquycq.html

now=$(date +%F); echo "$now"
来源：http://hz.bjfxy.top/gteqxtvdur.html

[R27] 算术展开
来源：http://hz.yvedp.cn/gtlojxjyxy.html

echo $((1 + 2 * 3))
来源：http://hz.tanke756.top/gtuvwltmik.html

[R28] 浮点运算
来源：http://hz.52xcode.cn/gtqbpolmlb.html

echo "scale=2; 10/3" | bc
来源：http://hz.jianghu66.top/gtrurkmezj.html

[R29] 定义函数
来源：http://hz.nanxuanxn.top/gtmxlvismk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.svipenyu.cn/gtymjdlbne.html

[R30] 函数返回状态码
来源：http://hz.fzhhl.top/gtnzvvukvj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gtltvymict.html

[R31] 局部变量
来源：http://hz.mhx1999.top/gtipgluxtb.html

f() { local x=1; echo "$x"; }
来源：http://hz.hammf.cn/gtkwsuxmnc.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtxeqkqgno.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtehvbneih.html

[R33] 捕获错误并提示行号
来源：http://hz.ppjwa.cn/gtotvxdpxt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.vqdsnc.cn/gtkrhffszk.html

[R34] 退出时清理
来源：http://hz.zhengqikj.top/gtktsxwhdp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jyoumei.cn/gtpvabsxap.html

[R35] 后台执行并等待
来源：http://hz.xuanzx.com/gtkspfkipl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.c1oappe.top/gtxizubiom.html

[R36] 并发执行多个任务
来源：http://hz.svipenyu.cn/gtzkoahxhd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cheryme.top/gtsjweofge.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gtuovqynzy.html

files=$(ls -1)
来源：http://hz.birdmap.top/gtjmsvhcxs.html

[R38] 管道串联
来源：http://hz.yongpay.top/gtlksrdbsp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ydjk.org.cn/gtvwppayeu.html

[R39] 重定向标准输出与错误
来源：http://hz.mhx1999.top/gtthntzcdl.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtgaxllgux.html

[R40] 追加写日志
来源：http://hz.feifeiyinyue.top/gtloacsdjj.html

echo "log" >> out.log
来源：http://hz.ydzc1.top/gtxhcnxpmf.html

[R41] 丢弃输出
来源：http://hz.gogol.net.cn/gtyeanmsmo.html

cmd >/dev/null 2>&1
来源：http://hz.redwolf501.top/gtqneqaoyd.html

[R42] 输入重定向
来源：http://hz.quarkkingdee.top/gtydwaxbzp.html

wc -l < a.txt
来源：http://hz.aizwys.cn/gtgoeecioq.html

[R43] 按名字查找文件
来源：http://hz.c1oappe.top/gtlsxhatgq.html

find . -name "*.log" -type f
来源：http://hz.0kj1m.cn/gtwryhorez.html

[R44] 按修改时间查找
来源：http://hz.nanxinkj.top/gtufyhprhr.html

find . -mtime -7 -type f
来源：http://hz.jinqigfzy.top/gtwlfwbzym.html

[R45] 批量删除
来源：http://hz.vqdsnc.cn/gtbthxgnzx.html

find . -name "*.tmp" -delete
来源：http://hz.zhixingplan.top/gtlmxiobkc.html

[R46] 递归替换文件内容
来源：http://hz.jiagoushi.top/gtlhzfzttd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhijiandao.cn/gtzbyuqwbf.html

[R47] sed 单行替换
来源：http://hz.zhiwuduotai.top/gtngtgeexw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shanyushiyangkeji.top/gttxobledq.html

[R48] awk 取指定列
来源：http://hz.yvedp.cn/gtzhwtzvqn.html

awk '{print $1, $3}' a.txt
来源：http://hz.daria6918.cn/gttzoebvcu.html

[R49] awk 带条件
来源：http://hz.gzhubu.top/gttrzygpoo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jlsjyb.cn/gtqlacmoei.html

[R50] awk 求和
来源：http://hz.jianghu66.top/gtmzofjmok.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gtxajbybgk.html

[R51] 排序去重取前几
来源：http://hz.jinqigufen.top/gtfrpggmrs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yongpay.top/gteriqnsfi.html

[R52] 统计行数
来源：http://hz.shanyushiyangkeji.top/gtrlsrwuqy.html

wc -l a.txt
来源：http://hz.zdqjudy.top/gtckuumiox.html

[R53] 查看文件头与实时尾
来源：http://hz.52xcode.cn/gtnqnjipyp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigufen.top/gtcynbsveb.html

[R54] 比较两个文件
来源：http://hz.snrcjt.cn/gtgeuudwgx.html

diff a.txt b.txt
来源：http://hz.wangshuangyany.cn/gtntcpsnfj.html

[R55] 压缩与解压
来源：http://hz.yj20258.top/gtoemkavft.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhiwuduotai.top/gtwdivunzu.html

[R56] 远程拷贝
来源：http://hz.zhixingplan.top/gtsekkdnau.html

scp file user@host:/path/
来源：http://hz.kuanghao11.cn/gtukcxpkug.html

[R57] 远程执行命令
来源：http://hz.redwolf501.top/gtwshvdefy.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtransnvth.html

[R58] 下载文件
来源：http://hz.sweek.top/gtkycwtnxo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.aizwys.cn/gtlpibdosm.html

[R59] 发 POST JSON
来源：http://hz.xinyue.icu/gtrlawraam.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtdvdjznoy.html

[R60] 只看 HTTP 状态码
来源：http://hz.hfpthk.cn/gtqhfyahog.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cdnleiting.top/gthynlaulz.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtynsrdphj.html

df -h;  du -sh *
来源：http://hz.ydjk.org.cn/gtpzwgtlgf.html

[R62] 找最占空间的文件
来源：http://hz.cdnleiting.top/gttladtpre.html

du -ah . | sort -rh | head -10
来源：http://hz.yonumen.top/gtgnqmzrco.html

[R63] 内存与进程
来源：http://hz.yongpay.top/gtyiyjzago.html

free -h;  ps aux | grep nginx
来源：http://hz.guowangkeji.top/gtbpdsfwxj.html

[R64] 结束进程
来源：http://hz.shanyushiyangkeji.top/gtpaqkzbcu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.meibo888.top/gtcupmbmob.html

[R65] 查看端口占用
来源：http://hz.shanyushiyangkeji.top/gtzthmystc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258888.top/gtgzinjlup.html

[R66] 定时任务
来源：http://hz.kuanghao11.cn/gtzgehzffy.html

crontab -e;  crontab -l
来源：http://hz.quarkkingdee.top/gttbtnwtcn.html

[R67] 生成随机十六进制串
来源：http://hz.mhx1999.top/gtzoxxiihl.html

openssl rand -hex 16
来源：http://hz.jqgufenzy.top/gtaxjgsmvo.html

[R68] 计算文件校验值
来源：http://hz.zhijiandao.cn/gtzazgkkfo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daxiang520.top/gtooebhpud.html

[R69] 生成随机密码
来源：http://hz.ybcxt.top/gtmsduwqnm.html

head -c 16 /dev/urandom | base64
来源：http://hz.fzhhl.top/gtvkhaqmeg.html

[R70] 时间戳与互转
来源：http://hz.zdqjudy.top/gtrnvnqgdj.html

date +%s;  date -d @1700000000
来源：http://hz.iojbl.cn/gtkktimtdf.html

[R71] 日期格式化
来源：http://hz.daxiang520.top/gtxbcclzxy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yvedp.cn/gtscpyzcqk.html

[R72] 等待端口就绪
来源：http://hz.chenjidiqi.icu/gtzwxprazo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.haohaochexian.top/gtkbmcmlph.html

[R73] 分割大日志
来源：http://hz.cashguo.top/gtrlmqwxha.html

split -l 1000 big.log part_
来源：http://hz.nanxinkj.top/gtyluddsva.html

[R74] 批量重命名
来源：http://hz.52xcode.cn/gtqftbvbch.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.quarkkingdee.top/gtsgtefkpu.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gtbqqeqqwa.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258888.top/gtezcsldzm.html

[R76] 使用临时文件
来源：http://hz.ydzc1.top/gtvzijidem.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtubdhdnbh.html

[R77] 读取用户输入
来源：http://hz.zhengqikj.top/gttdvldenm.html

read -rp "请输入: " ans
来源：http://hz.hnqzz.top/gtahxfevbr.html

[R78] 交互式菜单
来源：http://hz.zhoulong.xyz/gtjsacoxix.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhengqikj.top/gteqbppqzb.html

[R79] 解析命令行选项
来源：http://hz.sufxvd.cn/gtjylhsdba.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xuanzx.com/gtjidsxpdc.html

[R80] 查看脚本执行耗时
来源：http://hz.chenzaomai.com/gtdwcicsyl.html

time ./run.sh
来源：http://hz.yanxiufei.cn/gtzgdhxnfr.html

================================================================================
来源：http://hz.shzxlz.cn/gtbsmssjiy.html

S. C / C++ 专题
来源：http://hz.kuanghao11.cn/gtxrnfwiob.html

================================================================================
来源：http://hz.yj20258888.top/gtkcacmwgi.html

[S01] C：Hello World
来源：http://hz.wangshuangyany.cn/gtabuwbirp.html

#include <stdio.h>
来源：http://hz.zhijiandao.cn/gtynocpupk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jyoumei.cn/gtbougrpii.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangkeji.top/gtyroclkeq.html

int a = 10; printf("%d\n", a);
来源：http://hz.dianchejie.cn/gtwlplmkxn.html

[S03] C：读入整数
来源：http://hz.zhiwuduotai.top/gtbaipcgbk.html

int x; scanf("%d", &x);
来源：http://hz.dashuyun.cn/gtuvaldsqo.html

[S04] C：字符串复制
来源：http://hz.xingfuxueyuan.xyz/gtyfrmgcia.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnxiangtu.top/gtkjlgsvcx.html

[S05] C：字符串长度
来源：http://hz.ydzc1.top/gtedzbqmyk.html

strlen(s)
来源：http://hz.ppjwa.cn/gtfwazhyvc.html

[S06] C：字符串比较
来源：http://hz.cashguo.top/gttuhzvrbe.html

strcmp(a, b) == 0
来源：http://hz.mhx1999.top/gtqbfkuykh.html

[S07] C：数组遍历求和
来源：http://hz.chenjidiqi.icu/gtowkclxvr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.0kj1m.cn/gtvucwgxyk.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigfzy.top/gtiwdxbxna.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hysaishi.cn/gtjjznkhwh.html

[S09] C：结构体定义与初始化
来源：http://hz.aibaodan.cn/gtrlumubie.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.0kj1m.cn/gthsvhoqrp.html

[S10] C：指针与解引用
来源：http://hz.cashguo.top/gtxlovuweu.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigufen.top/gtqmusmahb.html

[S11] C：逐行读文件
来源：http://hz.hywenlv.cn/gtvvluigte.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yangfankeji.com/gtwatdoxtf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnxiangtu.top/gtiidzqbes.html

fclose(f);
来源：http://hz.nanxuanxn.top/gtcjmhkral.html

[S12] C：写文件
来源：http://hz.fengsongda.top/gtxhqpttll.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.mhx1999.top/gtouagdgzm.html

[S13] C：宏定义
来源：http://hz.jqgfzy.top/gtiufztfzo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhijiandao.cn/gtkpluujmo.html

[S14] C：枚举
来源：http://hz.aizwys.cn/gtsmwvgrqw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxinkj.top/gtfpgdueko.html

[S15] C：类型转换
来源：http://hz.0kj1m.cn/gtoswyshws.html

(double) a / b
来源：http://hz.sweek.top/gtmhnehckh.html

[S16] C：位操作置位
来源：http://hz.mhx1999.top/gtxgyfvjen.html

x |= (1 << 3);
来源：http://hz.xingfuxueyuan.xyz/gtxhyfysdh.html

[S17] C：安全拼接字符串
来源：http://hz.yuxming.cn/gtxgcmyyso.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gtcrxjwrng.html

[S18] C：命令行参数
来源：http://hz.fzhhl.top/gtavsgikey.html

int main(int argc, char **argv)
来源：http://hz.guannengcc.top/gtveigwhno.html

[S19] C：快速排序
来源：http://hz.shangyingyoupin.top/gtloamsumm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtiyoxzllo.html

[S20] C：二分查找
来源：http://hz.pycfn.com/gtuqppcwxc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtagamdlwj.html

[S21] C：字符类别判断
来源：http://hz.zhixingplan.top/gtviippbdg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xziqi.cn/gthqakkame.html

[S22] C：字符串转数字
来源：http://hz.xuetiantiany.cn/gtxborrufm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.c1oappe.top/gtzhmxbijv.html

[S23] C：随机数
来源：http://hz.jinqigufen.top/gtuxffvepm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yongpay.top/gtkbegtmdv.html

[S24] C：获取本地时间
来源：http://hz.yj20258.top/gtkpjzcwet.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cqqwz.cn/gteyjqqpsj.html

[S25] C：内存拷贝
来源：http://hz.xylfe.cn/gtdujmsgzz.html

memcpy(dst, src, n);
来源：http://hz.daria6918.cn/gtoigcetwj.html

[S26] C：内存清零
来源：http://hz.daxiang520.top/gtyawhzvle.html

memset(a, 0, sizeof a);
来源：http://hz.daria6918.cn/gtucveinjq.html

[S27] C：定义常量
来源：http://hz.shzxlz.cn/gtlikzuwha.html

const double PI = 3.14159;
来源：http://hz.52xcode.cn/gtnvwksnhp.html

[S28] C：静态变量
来源：http://hz.bjfxy.top/gtagqvrxyk.html

static int counter = 0;
来源：http://hz.hnqzz.top/gtnuhjpcly.html

[S29] C：变参函数
来源：http://hz.jinqigfzy.top/gttiaecxws.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yvedp.cn/gtagahxnrr.html

[S30] C：头文件保护
来源：http://hz.gogol.net.cn/gtjjrbfdhb.html

#ifndef X_H
来源：http://hz.yonumen.top/gtpcfewjoo.html

#define X_H
来源：http://hz.ywan-chungtsiang.top/gthxlpcefv.html

#endif
来源：http://hz.pengpengdd.cyou/gtonijyamh.html

[S31] C++：Hello World
来源：http://hz.zhijiandao.cn/gthpwxxlrl.html

#include <iostream>
来源：http://hz.kuanghao11.cn/gthqrbzfpp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.316326.xyz/gtjmewnoiz.html

[S32] C++：字符串
来源：http://hz.xuetiantiany.cn/gtqqehgxnz.html

std::string s = "hi";  s += "!";
来源：http://hz.shuidangran.top/gtickpmkqe.html

[S33] C++：vector 增删
来源：http://hz.chenzaomai.com/gtiqhuicxp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hammf.cn/gthhyiuoka.html

[S34] C++：遍历 vector
来源：http://hz.yongpay.top/gtczvajrol.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nwbrower.top/gtiabrkzdd.html


<!-- 参考信息 -->